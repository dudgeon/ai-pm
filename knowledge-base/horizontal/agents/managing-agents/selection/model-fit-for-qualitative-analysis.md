---
created: 2026-02-18
updated: 2026-02-18
tags: [knowledge, ai-pm]
status: draft
origin: sourced
featured: false
entry_type: insight
domain: horizontal
horizontal_domain: agents
lifecycle_phase: discover
---

# Model Fit for Qualitative Analysis Tasks

Claude, Gemini, and ChatGPT have meaningfully different strengths for qualitative research analysis. The right choice depends on whether you need depth, evidence, or stakeholder framing — and the tradeoffs are consistent enough to guide selection.

## The Pattern

Based on empirical comparison across 2,000+ hours of analysis testing (interviews, surveys, mixed qualitative data):

| Model | Best for | Key tradeoff |
|---|---|---|
| **Claude** | Depth + breadth; thorough coverage of themes while staying data-grounded | Doesn't filter — presents validated patterns and half-formed hypotheses with equal confidence; you do the filtering |
| **Gemini** | Strongly evidenced themes; fewer themes but better grounded; video analysis capability | Requires multiple prompts to get full coverage; chooses short quote snippets over longer passages |
| **ChatGPT** | Final stakeholder framing and communication; packaging findings for a specific audience | Most prone to synthesized "verbatim" quotes; least reliable for actual evidence; most creative (in both good and bad directions) |

**Default recommendation**: Use Claude for analysis work. You get breadth without pushing, and the tradeoff (unfiltered output) is manageable through the verification techniques.

## When Selection Matters

- **Exploratory discovery**: Claude — you want breadth to surface themes you might not have anticipated
- **Evidence-grounded decision**: Gemini — you need fewer themes, each with strong backing
- **Stakeholder communication**: ChatGPT — once you've verified your findings elsewhere, ChatGPT packages them most compellingly
- **Video/UX research with recorded sessions**: Gemini — unique capability for non-verbal behavior analysis

## Caveats

This comparison reflects model behavior at a specific point in time. Model capabilities shift with each release — specific rankings will change, but the underlying strengths (breadth vs. evidence vs. communication) may persist longer as they reflect different training emphases.

The techniques for accurate AI analysis (quote rules, context loading, calibration, verification) apply to all three models and are more important than model selection for most teams.

## Related

- [Quote Selection Rules for AI Analysis](../../../product-lifecycle/discover/quote-selection-rules-for-ai-analysis.md) — applicable regardless of model choice
- [Decision-Anchored Analysis Context](../../../product-lifecycle/discover/decision-anchored-analysis-context.md) — applicable regardless of model choice
- [AI Analysis Multi-Pass Verification](../../../product-lifecycle/discover/ai-analysis-multi-pass-verification.md) — applicable regardless of model choice

## Sources

**Caitlin Sullivan — "How to Do AI Analysis You Can Actually Trust" (Lenny's Newsletter, 2026-02-18)**
> "Here's what you need to know about each model: Claude: Best for thorough analysis with depth and nuance. Delivers more quotes and covers more ground with less pushing. The tradeoff: it gives you the whole brain dump, so themes aren't always 'proven' — you get breadth, not just the safe patterns."
> "Gemini: Best for highly evidenced themes and now video analysis. Gives you fewer themes but with stronger grounding."
> "ChatGPT: Best for final framing and stakeholder communication. Most creative of the three — including with 'verbatim quotes,' unfortunately. Least reliable for real evidence."
> "My recommendation: If you have a choice, use Claude for analysis work."

Unique contribution: Empirically grounded framework distinguishing model strengths as depth (Claude) vs. evidence (Gemini) vs. communication (ChatGPT); the insight that technique quality matters more than model selection for most teams.
