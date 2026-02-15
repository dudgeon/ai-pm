---
created: 2026-02-14
updated: 2026-02-14
template: templates/knowledge-entry.md
template_version: 5
tags: [knowledge, ai-pm, technique, shape, prototyping, vibe-coding]
status: draft
entry_type: technique
origin: sourced
featured: false
domain: product-lifecycle
lifecycle_phase: shape
component: Prototyping & Risk Reduction
project: ai-pm
---

# Parallel Prototyping for Clarity

## Summary

Instead of overthinking one design upfront, use AI's speed to launch multiple parallel prototypes with increasing specificity. Brain dump into the first project, get more specific in the second, add visual references in the third, attach actual code snippets in the fourth, compare all five. The cost is higher upfront (more credits, more sessions) but dramatically lower overall because you skip the long iteration tail of refining a single wrong-footed first attempt.

This inverts the traditional prototyping tradeoff. In pre-AI product development, prototypes were expensive enough that you carefully scoped each one. AI makes the marginal cost of a prototype near-zero, which means the optimal strategy shifts from "invest deeply in one path" to "explore the space broadly, then converge." The prototypes aren't throwaway wireframes — they're working software you can compare side-by-side to discover what you actually want.

The technique also solves a common problem with AI-assisted building: you often don't know what you want until you see what's possible. Parallel prototyping externalizes the exploration that would otherwise happen as an expensive inner loop of prompt-revise-prompt-revise within a single session.

## How to Apply

**When to use**: Early in the Shape phase when you're still discovering what the right solution looks like. Especially valuable when you have a general direction but haven't locked in the specifics of UI, architecture, or user flow.

**When not to use**: When requirements are well-specified and the implementation path is clear. If you already know exactly what you want, parallel exploration wastes time.

**The five-prototype sequence** (from Lazar Jovanovic's workflow):
1. **Brain dump** — throw everything at it, see what sticks
2. **More specific** — refine the prompt based on what you learned from #1
3. **Visual references** — attach design screenshots, UI inspirations
4. **Code snippets** — include actual component code or architecture patterns
5. **Compare all** — evaluate side-by-side, cherry-pick the best elements

**Key principles**:
- Each prototype uses a fresh context/session — don't accumulate debt from one into the next
- The sequence naturally increases in specificity, which mirrors how your own understanding sharpens
- Comparison across prototypes reveals preferences you couldn't articulate upfront
- Works with any AI building tool (Lovable, v0, Cursor, Claude Code)

**For AI PMs**: This pattern changes how you think about the shape-to-build handoff. Instead of writing a detailed spec first and building once, you can shape *through* building — using parallel prototypes as a discovery tool. The PRD becomes a synthesis of what you learned from prototypes, not a prerequisite for them.

## Sources

### From: [2026-02-08 Getting Paid to Vibe Code](../../sources/2026-02-08-vibe-coding-new-ai-job.md)
**Key quote**: "Instead of overthinking one design, start five parallel builds... This costs more up front but saves hundreds of credits and days of iteration later."
**Attribution**: Lazar Jovanovic (via Lenny Rachitsky)
**What this source adds**: The concrete five-prototype sequence and the practical insight that parallel exploration costs less than serial refinement. Jovanovic uses this in production work at Lovable — building internal tools and Shopify integrations — not just side projects.
**Links**: [Original](https://www.lennysnewsletter.com/p/getting-paid-to-vibe-code) | [Archive](../../sources/2026-02-08-vibe-coding-new-ai-job.md)

## Related

- [Shape the Product -- AI Disruption Profile](shape-the-product-ai-disruption.md) -- Prototyping is a Shape sub-skill; AI makes it dramatically cheaper, which enables this parallel approach
- [Context First Development](../build/context-first-development.md) -- Parallel prototyping is a way to *build* context: you learn what you need to specify by seeing multiple implementations
- [Interactive PRD Writing](../build/interactive-prd-writing.md) -- The PRD can become a synthesis of prototype learnings rather than a prerequisite
