---
created: 2026-02-18
updated: 2026-02-18
tags: [knowledge, ai-pm]
status: draft
origin: sourced
featured: false
entry_type: technique
domain: product-lifecycle
lifecycle_phase: discover
component: problem-signal-detection
---

# Few-Shot Calibration for Decision-Relevant Classification

When AI classifies qualitative data (interview responses, survey answers) into decision-relevant categories, provide concrete examples of each category level — including an explanation of *why* each example belongs there. This prevents AI from inventing its own interpretation of what each level means.

## The Technique

Build a labeled scale for your specific decision. For each level, provide:
1. A label describing the category
2. A concrete example from plausible participant data
3. An explanation of why that example belongs there

**Example: "Would a screen retain this churned user?" (5-point scale)**

```
SOLUTION FIT SCALE (calibrated for screen decision)

1 - SCREEN WOULD RETAIN: Explicit visibility/access pain during activity
  Example: "I check my phone 10 times per workout just to see my HR"
  Why this is a 1: Specific friction with current workaround. Screen
  directly solves this. High-value signal for screen investment.

2 - CHEAPER FIX WOULD RETAIN: Sounds screen-related but has lower-cost solution
  Example: "App was too clunky to check mid-workout, too many taps"
  Why this is a 2: Visibility complaint, but phone was present. App UX
  fix could solve this without hardware investment.

3 - ENGAGEMENT FIX NEEDED: Stopped using, screen wouldn't change that
  Example: "Just wasn't using it enough"
  Why this is a 3: Self-blame framing, no feature complaint. Screen
  doesn't fix habit formation.

4 - OPERATIONAL FIX NEEDED: Billing, support, reliability — not features
  Example: "Canceled 3 times and kept getting charged."
  Why this is a 4: Trust/process failure. Screen is irrelevant.

5 - UNRELATED COMPETITIVE LOSS: Left for alternative, no screen complaint
  Example: "Switched to Apple Watch, Whoop was fine"
  Why this is a 5: No negative language, no screen mention. Screen
  alone unlikely to win back.
```

## Why Examples Beat Descriptions

Descriptions of what a level *means* leave room for AI to apply its own interpretation. Examples do the teaching: they show AI the exact reasoning it should apply. With calibration, "22 people mentioned screens" becomes "8 would be retained by a screen, 6 just need app UX fixes, 8 are unrelated competitive losses" — a decision-relevant breakdown.

## Generalizing Beyond Feature Decisions

The same structure works for any classification task:
- Demand calibration for new offers (1 = would pay for this immediately → 5 = interesting but not a need)
- Feature request prioritization (1 = blocking, core use case → 5 = nice-to-have, power user only)
- Feedback quality scoring (1 = specific, actionable → 5 = vague, unactionable)
- Churn reason classification (customer service → pricing → product gap → competitive loss)

Build the scale once for a given decision context, then reuse across analyses.

## When to Apply

- Feature investment decisions driven by interview or survey data
- Churn analysis where you need to understand which reasons would be addressed by a specific fix
- Prioritization exercises across multiple customer requests
- NPS driver analysis where open-ends need to be classified by type of issue

## Related

- [Decision-Anchored Analysis Context](decision-anchored-analysis-context.md) — sets the decision frame that makes the scale meaningful
- [Quote Selection Rules for AI Analysis](quote-selection-rules-for-ai-analysis.md) — ensures evidence behind classifications is real
- [Multi-Pass AI Analysis Verification](ai-analysis-multi-pass-verification.md) — validates classification decisions after the fact

## Sources

**Caitlin Sullivan — "How to Do AI Analysis You Can Actually Trust" (Lenny's Newsletter, 2026-02-18)**
> "The examples above do the teaching. I'm not saying, 'This is what good output looks like.' I'm saying, 'This is good output, and here's why I labeled it this way, so you can follow my process.'"
> "Without clarity like this, the model invents its own interpretation of what 'screen-related churn reasons' look like — and it won't always match yours."
> "You'll spend a few extra minutes building a scale for your context, but you can reuse it across analyses."

Unique contribution: Explicit framing of "examples teach, descriptions don't"; the full 5-point scale template with rationale-per-level; the insight that the *why* explanation is what makes few-shot calibration work.
