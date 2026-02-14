---
created: 2026-02-05
updated: 2026-02-13
tags: [project, ai-pm-craft, product-management, learning]
status: active
domain: professional-development
pattern: domain-source-synthesis
source_types: [article, video, podcast, book-chapter, organic, note]
---

# AI PM Craft

A knowledge base for AI-augmented product management — how PMs use AI tools effectively and how product organizations adapt to AI-native ways of working. Every idea is traceable back to its sources with quotes, context, and links.

## Structure

```
ai-pm-craft/
├── sources/           Source material with full attribution and reading status
├── knowledge-base/    Extracted knowledge organized by domain
│   ├── product-lifecycle/{phase}/       Mapped to six lifecycle phases (vertical)
│   ├── horizontal/                      Cross-cutting knowledge areas (stack by delivery mechanism)
│   │   ├── context/                     Knowledge infrastructure (discoverability, KM)
│   │   ├── prompting/                   Portable techniques (any chat window)
│   │   ├── gems-and-gpts/              Packaged, shareable AI tools (GPTs, Gems)
│   │   └── agents/                      Autonomous AI participants (lifecycle, skills)
│   └── ai-adoption/                     Org change and adoption
└── meta/              Project ontology, taxonomy, and lifecycle framework
```

## Sources

Source material is the raw input — articles, podcasts, newsletters, and organic experience. Each source gets a structured note with attribution, key quotes, and extracted ideas.

**Pipeline**: `unread` → `reading` → `read` → `processed`

Browse all sources and their status in the [Source Registry](sources/), or jump to [unread sources](sources/#unread).

## Knowledge Base

Knowledge entries are ideas extracted from sources and organized by domain. Entries improve over time as more sources corroborate them.

**Entry types**: `technique` · `mental-model` · `insight`
**Entry status**: `draft` → `solid` (multiple sources) → `canonical` (vetted, teachable)

Browse all entries in the [Knowledge Map](knowledge-base/README.md).

## Taxonomy & Meta

Classification rules, lifecycle framework, and entry templates live in `meta/`. See [taxonomy.md](meta/taxonomy.md) for how entries are categorized.

---

## Status

Early stage. 25 sources captured, 3 fully processed into 14 knowledge entries (all draft). 19 unread sources in the queue. Entries span Build, Shape, Context, Prompting, Agents, and AI Adoption. Gems & GPTs layer awaiting source processing to populate.

---

## Related

- [Professional Development](../README.md) — Parent domain
- Context: `context/professional.md`

---

[← Back to Professional Development](../README.md)
