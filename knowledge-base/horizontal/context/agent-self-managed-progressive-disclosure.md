---
created: 2026-02-18
updated: 2026-02-18
tags: [knowledge, ai-pm]
status: draft
origin: sourced
featured: false
entry_type: technique
domain: horizontal
horizontal_domain: context
---

# Agent-Self-Managed Progressive Disclosure

Agents can manage their own context disclosure — deciding what to load, what to surface in navigation, and how to reorganize their knowledge as it grows — using the same filesystem primitives they use for everything else. This extends progressive disclosure from a design pattern imposed by humans into a dynamic capability agents maintain themselves.

## The Pattern

Agent memory is organized as a filesystem the agent can read and modify:

1. **Filetree as navigation signal** — The directory hierarchy and file names are always in the system prompt, even when file contents aren't loaded. Agents use this as a navigational index to decide what to read.

2. **Frontmatter as content preview** — Files carry YAML frontmatter describing their contents, so agents can evaluate relevance without loading the full file.

3. **`system/` directory for always-loaded context** — A designated folder for files that are always fully loaded into the system prompt regardless of task. Agents move files in/out of `system/` as they determine what should be persistent context vs. on-demand.

4. **Active reorganization** — Agents can restructure the filetree itself: renaming folders to make navigation clearer, splitting large files, merging duplicates, and updating frontmatter descriptions as their understanding evolves.

## Why This Matters

Most progressive disclosure designs are static: a human architect decides the hierarchy and files at setup time. Agent-self-managed disclosure is dynamic — the knowledge structure evolves as the agent learns, reflecting its current understanding of what's important and how concepts relate.

This is analogous to how a human knowledge worker organizes their files over time: initial structure → accumulated experience → reorganization to reflect deeper understanding. Agents can do this cycle explicitly and verifiably.

## Relationship to Existing Patterns

This extends [Three-Layer Context Disclosure](three-layer-context-disclosure.md) (index → summary → full content) by making the layer management dynamic rather than static. The filetree serves as the index layer; frontmatter serves as the summary layer; and full file content is the on-demand layer — but agents actively maintain all three.

The `system/` directory concept directly parallels the `@import` pattern in `CLAUDE.md`: files designated for always-on loading regardless of task context.

## Design Heuristic: 15–25 Files

Letta's defragmentation skill targets 15–25 focused files as the optimal granularity for agent-readable knowledge. Too many files create navigation overhead; too few create files too large and diffuse to be useful. Worth using as a calibration target when designing agent knowledge structures.

## Related

- [Three-Layer Context Disclosure](three-layer-context-disclosure.md) — the underlying progressive disclosure pattern this extends
- [Filesystem as Retrieval Architecture](filesystem-as-retrieval-architecture.md) — filesystem as a legitimate retrieval system
- [Agent Memory Lifecycle Skills](../agents/system-design/skills/agent-memory-lifecycle-skills.md) — the built-in skills (defragment, reflect) that maintain the knowledge structure over time

## Sources

**Letta — "Introducing Context Repositories: Git-based Memory for Coding Agents" (Letta Blog, 2026-02-12)**
> "Files in the context repository are designed for progressive disclosure, similar to patterns recommended for agent skills (references Anthropic's 'Effective Context Engineering for AI Agents'). The filetree structure is always in the system prompt, so folder hierarchy and file names act as navigational signals."
> "Because agents have programmatic access to the repository, they can manage their own progressive disclosure by reorganizing the file hierarchy, updating frontmatter descriptions, and moving files in and out of system/ to control what's pinned to context as they learn over time."

Unique contribution: Demonstrating that agents can actively manage their own progressive disclosure structure, not just consume a human-designed one; the `system/` directory as a first-class always-loaded context primitive.
