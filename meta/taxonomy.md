---
created: 2026-02-08
updated: 2026-02-08
tags: [meta, ai-pm-craft, taxonomy]
status: active
---

# AI PM Craft — Taxonomy

Canonical reference for classifying knowledge entries. Used by the source processing skill and knowledge entry template.

For full phase lineage, component descriptions, and AI-PM emphasis, see [Lifecycle Framework V2](lifecycle-framework-v2.md).

---

## Three Domains

Every knowledge entry belongs to exactly one domain.

| Domain | Folder | What belongs here |
|---|---|---|
| **Product Lifecycle** | `knowledge-base/product-lifecycle/{phase}/` | Techniques and insights that augment a specific stage of building product |
| **Horizontal** | `knowledge-base/horizontal/` | Patterns that cut across the lifecycle — prompting, context engineering, writing, workflow design |
| **AI Adoption** | `knowledge-base/ai-adoption/` | How organizations and individuals adapt to AI-native ways of working — scaling expertise, org change, driving adoption |

### Classification test

1. **Does this technique augment a specific lifecycle phase?** → Product Lifecycle (file under the phase)
2. **Is it a portable skill applicable regardless of phase?** → Horizontal
3. **Is it about bringing others along or changing how teams/orgs work?** → AI Adoption

---

## Product Lifecycle Phases

Six phases, each with named components. Entries sit flat in the phase folder; the `component` frontmatter field records the most specific applicable component.

### 1. Discover

*What problems are worth solving?*

| Component | Slug | Description |
|---|---|---|
| Problem Signal Detection | `problem-signal-detection` | Detecting unmet needs from data, support, sales, and customer contact |
| Market & Competitive Intelligence | `market-competitive-intelligence` | Competitive analysis, market sizing, trend monitoring |
| Opportunity Prioritization | `opportunity-prioritization` | Ranking and managing the space of possible problems |
| Problem Brief | `problem-brief` | Concise articulation of the problem, who it affects, why now |

### 2. Frame

*What does success look like, and what's the bet?*

| Component | Slug | Description |
|---|---|---|
| Stakeholder Intent Alignment | `stakeholder-intent-alignment` | Refining intent, securing sponsorship, shared understanding |
| Success Criteria & Business Case | `success-criteria-business-case` | KPIs, financial modeling, defining the objective function |
| Roadmap Definition | `roadmap-definition` | Outcome-based roadmapping, strategic sequencing, scoping |

### 3. Shape

*What solution takes form, and for whom?*

| Component | Slug | Description |
|---|---|---|
| Persona & Journey Mapping | `persona-journey-mapping` | User models, behavioral archetypes, JTBD framing |
| Prototyping & Risk Reduction | `prototyping-risk-reduction` | Wireframes, prototypes, fat-marker sketches, assumption testing |
| Go-to-Market Planning | `gtm-planning` | Positioning, messaging, channel strategy, pricing |

### 4. Build

*How do we ship with clarity and conviction?*

| Component | Slug | Description |
|---|---|---|
| Feature Specification Writing | `feature-specification-writing` | PRDs, specs, technical design documents |
| User Story & Acceptance Criteria | `user-story-acceptance-criteria` | Story decomposition, acceptance criteria, story mapping |
| Stakeholder Communication | `stakeholder-communication` | Status updates, cross-functional coordination, expectation management |
| Scope & Priority Tradeoffs | `scope-priority-tradeoffs` | Scope negotiations, circuit breakers, quality/speed tradeoffs |

### 5. Release

*How do we put this into the world deliberately?*

| Component | Slug | Description |
|---|---|---|
| Release Readiness Assessment | `release-readiness-assessment` | Go/no-go evaluation, quality gates, support readiness |
| Phased Rollout Strategy | `phased-rollout-strategy` | Feature flags, canary deploys, segment-based rollouts |
| Release Communications | `release-communications` | Changelogs, release notes, stakeholder notifications |
| Launch Marketing & Enablement | `launch-marketing-enablement` | Launch campaigns, sales enablement, customer success briefings |

### 6. Measure

*Did it work, and what do we do next?*

| Component | Slug | Description |
|---|---|---|
| KPI & Outcome Monitoring | `kpi-outcome-monitoring` | North Star dashboards, OKR reviews, post-launch accountability |
| Customer Feedback Collection | `customer-feedback-collection` | NPS/CSAT, surveys, support themes, interview programs |
| Experiment Design & Analysis | `experiment-design-analysis` | A/B tests, statistical rigor, acting on results |
| End-of-Life & Deprecation | `end-of-life-deprecation` | Sunsetting, migration paths, deprecation communication |

---

## Entry Types

| Type | Slug | What it captures |
|---|---|---|
| Technique | `technique` | A named method, practice, or procedure |
| Mental Model | `mental-model` | A framework for thinking about a class of problems |
| Insight | `insight` | An observation, principle, or non-obvious pattern |

## Entry Status

| Status | Meaning | Promotion criteria |
|---|---|---|
| `draft` | Initial capture from one source | — |
| `solid` | Supported by multiple sources, well-articulated | Corroboration from a second independent source |
| `canonical` | Thoroughly vetted, teachable | Could teach this to someone; no open questions |

## Entry Origin

| Origin | Meaning |
|---|---|
| `sourced` | Extracted from external sources |
| `organic` | From personal experience |
| `both` | Originated organically, later found external validation |

---

## Frontmatter Reference

Knowledge entry frontmatter fields for taxonomy:

```yaml
# Required
entry_type: technique | mental-model | insight
domain: product-lifecycle | horizontal | ai-adoption

# Required for product-lifecycle entries
lifecycle_phase: discover | frame | shape | build | release | measure
component: <component-slug from tables above>

# Optional
featured: true  # Worth championing organizationally
```

---

## Placement Rules

1. **Most specific component wins.** If an entry clearly maps to a component, tag it there. If it spans multiple components within a phase, use the primary one and note connections in Related.
2. **Phase-level is OK.** If an entry fits a phase but not a specific component, omit the `component` field and file it in the phase folder.
3. **Cross-phase entries go horizontal.** If an entry applies across 3+ phases, it's probably a horizontal skill, not a lifecycle entry.
4. **When in doubt, ask.** Don't force-fit entries into the taxonomy. Flag uncertain placements for review.
5. **Screen for adoption.** Sources often embed change management insights alongside craft techniques. Extract these separately into ai-adoption.
