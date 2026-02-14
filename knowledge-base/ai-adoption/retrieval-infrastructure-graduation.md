---
created: 2026-02-14
updated: 2026-02-14
template: templates/knowledge-entry.md
template_version: 4
tags: [knowledge, ai-pm, mental-model, ai-adoption, infrastructure, retrieval, knowledge-management]
status: draft
entry_type: mental-model
origin: sourced
featured: false
domain: ai-adoption
project: ai-pm
---

# Retrieval Infrastructure Graduation

## Summary

Organizations don't need to solve agent memory/retrieval all at once. There's a natural graduation path from zero infrastructure to full knowledge graph, and the filesystem conventions at each tier are designed to remain useful — and become *better* — at higher tiers. The key insight: start with what works everywhere (files), and layer on capabilities only when scale demands it.

- **Tier 1 (Baseline)**: Filesystem primitives — `grep`, `find`, `ls`, `head`. Directory structure serves as the index. Frontmatter provides metadata. Git provides temporal tracking. Works in any agent that can read files. Zero infrastructure beyond a git repo.
- **Tier 2 (Enhanced)**: MCP server with semantic search (e.g., BrainStem, Claude-Mem). Adds vector embeddings for fuzzy matching, relevance ranking, and cross-document discovery. The filesystem conventions (frontmatter, READMEs) make search results richer because there's structured metadata to surface.
- **Tier 3 (Advanced)**: Knowledge graph with entity extraction (e.g., Graphiti/Zep, Neo4j). Adds entity-relationship triples, temporal validity tracking, multi-hop reasoning, and automatic conflict detection. The structured frontmatter from tiers 1-2 can be ingested directly into the graph without reformatting.

The graduation path matters because it prevents two common failure modes: (1) over-investing in infrastructure before the knowledge base has enough content to justify it, and (2) building filesystem conventions that work at tier 1 but can't be leveraged by higher tiers.

## How to Apply

**When to use**: When making infrastructure decisions for agent knowledge/memory systems, when advising teams on where to start, or when evaluating whether to invest in embedding search or graph databases. The model provides a principled answer to "should we build a knowledge graph?" — usually "not yet, and here's what to do first."

**When not to use**: When the organization already has graph database expertise and the scale clearly warrants it (thousands of entities with complex interrelationships, multiple agents reasoning across the same knowledge, temporal accuracy is critical).

**Decision criteria for graduation**:
- **Stay at Tier 1** when: <500 documents, single team, grep finds what you need most of the time, enterprise policy restricts external services
- **Graduate to Tier 2** when: grep misses are frequent, cross-domain discovery matters, fuzzy matching would help, you need to search from non-filesystem clients (mobile, web)
- **Graduate to Tier 3** when: you have thousands of entities with interrelationships, multiple agents/users need to reason across the same knowledge, temporal accuracy is critical (what was true at a specific point in time), multi-hop reasoning is a common query pattern

**For AI PMs**: This mental model is directly applicable to product roadmapping for agent-powered features. It provides a principled argument against premature infrastructure investment and a clear set of graduation criteria. When stakeholders ask "shouldn't we build a knowledge graph?", this framework gives you a structured answer grounded in actual implementation patterns.

## Sources

### From: [2026-02-14 Progressive Disclosure & Context Graphs](../../sources/2026-02-14-progressive-disclosure-context-graphs.md)
**Key quote**: "The filesystem conventions (frontmatter, READMEs, directory structure) are designed to work at tier 1 but become *better* with tiers 2-3. Nothing in the base pattern precludes future enhancement."
**Attribution**: Research synthesis drawing on Letta Context Repositories, Graphiti/Zep, Claude-Mem, and BrainStem implementations
**What this source adds**: Defines the three tiers explicitly, provides graduation criteria, and documents the critical design principle that conventions at each tier should be forwards-compatible with higher tiers. Also provides the honest assessment that most individual/small-team knowledge bases don't yet need tier 3.
**Links**: [Archive](../../sources/2026-02-14-progressive-disclosure-context-graphs.md)

## Related

- [Filesystem as Retrieval Architecture](../horizontal/context/filesystem-as-retrieval-architecture.md) — The mental model underlying tier 1. Understanding why filesystem-only retrieval works is prerequisite to understanding when to graduate beyond it.
- [Data Silos Block Enterprise Agent Adoption](data-silos-block-agent-adoption.md) — Related adoption barrier: even with tier 3 infrastructure, fragmented data across SaaS tools limits agent effectiveness. The graduation path assumes data accessibility.
- [Self-Maintaining Knowledge Bases](self-maintaining-knowledge-bases.md) — Knowledge base maintenance patterns apply at every tier. Self-maintaining properties (corrections → persistent knowledge) complement infrastructure graduation.
