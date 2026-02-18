---
created: 2026-02-18
updated: 2026-02-18
tags: [knowledge, ai-pm]
status: draft
origin: sourced
featured: false
entry_type: technique
domain: horizontal
horizontal_domain: agents
---

# Concurrent Agent Memory via Git Worktrees

Multiple subagents can write to the same shared memory repository simultaneously by giving each subagent its own git worktree. Changes merge through standard git operations, enabling "memory swarms" — parallel subagents that process information and write memory concurrently without conflicts.

## The Pattern

1. A shared context repository serves as the canonical memory store for an agent ensemble
2. When multiple subagents need to write memory simultaneously, each gets an isolated git worktree — a separate working directory sharing the same git history
3. Each subagent writes to its worktree independently; there's no locking or coordination overhead during the write phase
4. Changes merge back into the main branch through standard git operations, with conflict resolution handling divergent writes

## Why This Matters

Most multi-agent memory systems treat memory as a single-writer resource. This becomes a bottleneck when:
- Initializing an agent that needs to learn from a large corpus (session histories, documents, past work)
- Running a "memory swarm" that processes many inputs in parallel and writes learnings simultaneously
- Operating multiple specialist agents that each maintain domain-specific memory

Git worktrees solve this by applying version control's existing mechanism for parallel isolated development to agent memory. The concurrency model (branch → write → merge) is battle-tested; the insight is applying it to memory rather than code.

## Primary Use Case: Agent Initialization at Scale

Letta's `/init` tool bootstraps new agents by distributing history processing across concurrent subagents. Each subagent reflects on a slice of session history in its own worktree, then results merge into the main memory. What would be sequential (and slow) becomes parallel:

```
Main memory repo
├── subagent-1 worktree → processes history slice 1-20 → commits learnings
├── subagent-2 worktree → processes history slice 21-40 → commits learnings
├── subagent-3 worktree → processes history slice 41-60 → commits learnings
└── merge → unified agent memory with full history synthesis
```

## Relationship to Single-Agent Patterns

For single-agent systems, this pattern isn't needed — a single agent reads and writes sequentially. The pattern becomes relevant when:
- Multiple agents collaborate on shared memory
- Parallelizing a task that involves memory writes (e.g., processing a large corpus on initialization)
- Running background memory maintenance (reflection, defragmentation) concurrent with active agent execution

## Related

- [Git-Versioned Agent Memory](git-versioned-agent-memory.md) — the foundation that makes worktrees viable
- [Agent Memory Lifecycle Skills](../skills/agent-memory-lifecycle-skills.md) — the initialization skill that uses this pattern
- [Filesystem as Agent State](filesystem-as-agent-state.md) — the base architecture

## Sources

**Letta — "Introducing Context Repositories: Git-based Memory for Coding Agents" (Letta Blog, 2026-02-12)**
> "Memory formation and learning in agents has been single-threaded — no mechanism to coordinate concurrent writes to memory. Git changes this by giving each subagent an isolated worktree, allowing multiple subagents to process and write to memory concurrently, then merge their changes back through git-based conflict resolution."
> "The /init tool can optionally learn from existing Claude Code and Codex histories by fanning out processing across concurrent subagents. Each subagent reflects on a slice of history in its own worktree, and results are merged back into 'main' memory."

Unique contribution: Identifying multi-agent memory coordination as a previously single-threaded bottleneck; git worktrees as the concurrency solution; the initialization use case as the primary application.
