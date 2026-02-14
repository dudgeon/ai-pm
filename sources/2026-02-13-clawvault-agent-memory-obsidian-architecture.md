---
title: "ClawVault: Solving Agent Memory With Obsidian-Style Architecture"
created: 2026-02-14
updated: 2026-02-14
template: templates/source.md
template_version: 3
tags: [source, ai-pm]
status: unread
source_type: article
source_url: "https://x.com/sillydarket/status/2022394007448429004"
archive_url: "domains/professional-development/ai-pm/sources/2026-02-13-clawvault-agent-memory-obsidian-architecture.md"
author: "Pedro (@sillydarket)"
published: 2026-02-13
discovered: 2026-02-14
summary: "Open-source agent memory architecture (ClawVault) modeled on Obsidian's filesystem approach. Plain markdown with YAML frontmatter outperformed purpose-built memory infrastructure (74% vs 68.5% on LoCoMo benchmark). Key patterns: typed memory taxonomy (decisions, preferences, relationships, commitments, lessons), wiki-link knowledge graphs for associative retrieval, priority-tagged observational memory with budget-aware context injection, vault index for efficient lookup. Zero cloud dependency — agent memory as inspectable, auditable, editable human-readable files."
domain: professional-development
project: ai-pm
---

# ClawVault: Solving Agent Memory With Obsidian-Style Architecture

**By**: Pedro (@sillydarket), Versatly
**Source**: [X Article](https://x.com/sillydarket/status/2022394007448429004)
**Type**: article (X long-form)

## Summary

ClawVault is an open-source memory architecture for AI agents built on the insight that plain markdown files in folders outperform purpose-built memory infrastructure. Benchmarked against LoCoMo, a simple filesystem with markdown scored 74% vs 68.5% for specialized memory tools (Mem0, Zep, vector DBs, custom RAG). The architecture mirrors Obsidian's approach: markdown files with YAML frontmatter, wiki-links for connections, and folder hierarchies for organization.

## Key Concepts

### Typed Memory Taxonomy
Not all memories are equal. ClawVault enforces memory types — decisions, preferences, relationships, commitments, lessons, handoffs — stored in corresponding folders. This enables structured retrieval ("show me all decisions from last month") that flat storage can't support.

### Wiki-Link Knowledge Graph
Agent memories use `[[entity-name]]` wiki-links, creating a traversable knowledge graph. When asked about a project, the agent follows links to find related decisions, people, commitments, and lessons — associative memory via graph traversal.

### Priority-Tagged Observational Memory
Conversations compressed into priority-tagged observations (critical/notable/background). On wake, the agent loads critical observations first, then fills remaining context budget with lower-priority items. Budget-aware context injection ensures important memories always make the window.

### Vault Index Pattern
A single index file listing every note with a one-line description. Agent scans the index before deciding what to read — dramatically more efficient than embedding search for most queries. Index as table of contents; embeddings as search engine. Use both.

### LLM Compression Caveat
LLMs rewrite keywords during summarization, breaking downstream pattern matching. Fix: regex-based priority enforcement AFTER LLM compression. Trust LLM for compression quality, not classification accuracy.

### Filesystem Benchmark Result
Plain markdown files with grep/search scored 74.0% on LoCoMo vs 68.5% for specialized memory tools. LLMs already know how to work with files from training data — fighting that instinct with specialized APIs is counterproductive.

## Notes

- Strong resonance with home-brain architecture and the Mernit/Openclaw "filesystem as state" source
- The typed memory taxonomy maps almost directly to home-brain's domain/context structure
- Vault index pattern is what our source registry and domain READMEs already do — validate agents' memory using human-readable indexes
- Priority-tagged observational memory is a formalization of what CLAUDE.md's @import pattern does: critical context auto-loads, reference material is on-demand
- The "human knowledge management and agent memory management are the same problem" thesis is the core argument of this entire ai-pm domain
- ClawVault is open source: https://github.com/Versatly/clawvault

## Raw Content

Every AI agent has the same fatal flaw: context death. The moment a session ends, everything dies — decisions, preferences, relationships, project context. The team at Versatly spent months on this problem, building ClawVault, an open-source memory architecture.

They benchmarked every agent memory solution they could find (Mem0, Zep, vector databases, custom RAG pipelines) against LoCoMo. Specialized memory tools scored 68.5%; a simple filesystem with markdown files scored 74.0%.

The Obsidian insight: notes are just files. No proprietary database, no cloud lock-in. Markdown files in folders with YAML frontmatter for metadata, wiki-links for connections, and emergent graph structure. ClawVault stores every memory as a markdown file with YAML frontmatter — simultaneously a ClawVault document, an Obsidian note, and a plain text file.

Memory types matter: decisions, preferences, relationships, commitments, lessons. Every memory is typed because structured retrieval requires structured storage. The category system maps to Obsidian folders (decisions/, people/, lessons/, projects/, commitments/, preferences/, handoffs/).

Wiki-links inside notes create a knowledge graph — the same graph visible in Obsidian's graph view, but navigable programmatically by the agent as associative memory.

Observational memory compresses conversations into priority-tagged observations (critical, notable, background). On wake, the agent loads critical first, then fills remaining context budget. Key caveat: LLMs rewrite keywords during compression, so regex-based priority enforcement runs AFTER LLM compression.

The vault index pattern: a single file listing every note with a description. Agent scans this first — more efficient than embedding search for most queries. Index is table of contents; embeddings are search engine.

Zero cloud dependency. No telemetry, no sync service. Agent memories live on the filesystem. The thesis: human knowledge management and agent memory management are the same problem, requiring typed storage, associative linking, priority-based retrieval, signal-preserving compression, and zero platform lock-in.
