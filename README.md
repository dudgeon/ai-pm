---
created: 2026-02-05
updated: 2026-02-08
tags: [project, ai-pm-craft, product-management, learning]
status: active
domain: professional-development
---

# AI PM Craft

A knowledge base for AI-augmented product management — how PMs use AI tools effectively and how product organizations adapt to AI-native ways of working. Every idea is traceable back to its sources with quotes, context, and links.

## Structure

```
ai-pm-craft/
├── sources/           Source material with full attribution and reading status
├── knowledge-base/    Extracted knowledge organized by domain
│   ├── product-lifecycle/{phase}/   Mapped to six lifecycle phases
│   ├── horizontal/                  Cross-cutting skills
│   └── ai-adoption/                 Org change and adoption
└── meta/              Project ontology, taxonomy, and lifecycle framework
```

**Sources**: `unread` → `reading` → `read` → `processed` (see `sources/_index.md`)
**Entries**: `draft` → `solid` (multiple sources) → `canonical` (vetted, teachable)
**Entry types**: `technique` · `mental-model` · `insight`
**Taxonomy reference**: `meta/taxonomy.md`

---

## Knowledge Map

### Product Lifecycle

Six phases. Entries sit flat within phase folders; the `component` frontmatter field records the most specific applicable component. See `meta/lifecycle-framework-v2.md` for full phase lineage and AI-PM emphasis.

#### Discover

*What problems are worth solving?*
Components: Problem Signal Detection · Market & Competitive Intelligence · Opportunity Prioritization · Problem Brief

*No entries yet.*

#### Frame

*What does success look like, and what's the bet?*
Components: Stakeholder Intent Alignment · Success Criteria & Business Case · Roadmap Definition

*No entries yet.*

#### Shape

*What solution takes form, and for whom?*
Components: Persona & Journey Mapping · Prototyping & Risk Reduction · Go-to-Market Planning

*No entries yet.*

#### Build

*How do we ship with clarity and conviction?*
Components: Feature Specification Writing · User Story & Acceptance Criteria · Stakeholder Communication · Scope & Priority Tradeoffs

- [[interactive-prd-writing]] — Templatized rule files + AI follow-up questions for thorough PRDs `build/feature-specification-writing`
- [[task-list-generation-for-observability]] — Decomposing PRDs into nested task lists for observability and control `build/user-story-acceptance-criteria`
- [[context-first-development]] — The biggest mistake in AI-assisted dev is rushing past context `build`

#### Release

*How do we put this into the world deliberately?*
Components: Release Readiness Assessment · Phased Rollout Strategy · Release Communications · Launch Marketing & Enablement

*No entries yet.*

#### Measure

*Did it work, and what do we do next?*
Components: KPI & Outcome Monitoring · Customer Feedback Collection · Experiment Design & Analysis · End-of-Life & Deprecation

*No entries yet.*

---

### Horizontal Product & Knowledge Work

Patterns that cut across the product lifecycle — prompting techniques, writing workflows, context engineering, workflow design.

- [[be-100x-more-specific]] — Forces AI past vague principles into concrete, actionable standards
- [[my-job-your-job-role-delineation]] — Explicit human/AI responsibility partitioning
- [[deliberate-context-selection]] — Hand-picking files for LLM context vs. relying on automatic context
- [[ai-as-writing-coach]] — Structured workflow: thesis validation → blind spots → restructuring
- [[stepwise-task-execution]] — One-task-at-a-time execution with pause-and-approve checkpoints

### AI Adoption & Change Management

How organizations and individuals adapt to AI-native ways of working — scaling expertise, restructuring teams, driving adoption.

- [[reverse-engineer-judgment-into-ai]] — Have AI discover your implicit criteria, encode into reusable evaluator
- [[scale-manager-expertise-with-ai]] — Automate "0-to-60%" feedback so managers focus on high-leverage work

---

## Status

Early stage. 11 sources captured, 2 fully processed into 10 knowledge entries (all draft). 7 unread sources in the queue. Current entries cluster in Build, Horizontal, and AI Adoption — other lifecycle phases will populate as more sources are processed.

---

## Related

- [[professional-development]] — Parent domain
- Context: `context/professional.md`

---

[← Back to Professional Development](../README.md)
