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

# Decision-Anchored Analysis Context

Before prompting AI to analyze qualitative research data, load four specific context components that anchor the analysis to your decision. Without this framing, AI defaults to generic consensus-finding — themes that could describe any product in your category, which can't resolve the specific decision you're trying to make.

## The Four Components

**1. Project context** — Scope and stakes
> "We're exploring whether to add a screen to Whoop. This is a major hardware decision. These are 10 interviews with churned users."

Not just "doing customer research" — specific decision, specific data, specific stakes.

**2. Business goal** — The decision you're actually making
> "Determine if a screen would: (a) win back churned users, (b) fail to solve the core problems of churned users, or (c) come with other requirements to succeed."

Framing as a decision with explicit options forces AI to weight evidence toward answering *your* question, not the question it assumes you're asking.

**3. Product context** — Domain knowledge
> "Current: No screen, all data via app. Value prop is focus during activity. Key competitors with screens: Apple Watch, Garmin, Suunto. Without screen: Oura. Core tension: Is screenless a limitation for key audiences, or a request from audiences we shouldn't focus on?"

Without this, "I want to see my data" is interpreted generically. With it, AI understands that statement in the context of a screenless wearable competing against Apple Watch — a completely different interpretation.

**4. Participant overview** — Who's speaking
> "All participants are CHURNED users. Lifetime with Whoop: 6 months to 2 years."

"I need real-time data" from a churned Garmin switcher means something different than the same words from a loyal user who's never tried a competitor. AI can only weight evidence correctly if it knows who the evidence is coming from.

## For Survey Data: Add a Fifth Component

**Data structure** — Column disambiguation
> "Column A (response_id): Ignore. Column B (product_tier): 'one'/'peak'/'life' — use for segmentation. Column C (response): Customer's voice — primary analysis target. Column D (status): Internal tag — 0 = churned, 1 = active."

AI treats every column as signal unless told otherwise. Internal tracking codes, timestamps, and metadata columns get analyzed alongside customer voice without explicit instruction.

## Why Generic Context Fails

Three lines of objectives + vague background ("we're doing research on our wearable product") primes AI to find generic patterns — and LLMs have training priors that reinforce this (if it's seen thousands of wearables studies where price is the #1 theme, it weights toward price even if your data doesn't support it).

The goal: force AI to find evidence that can answer the specific decision in your context, with the specific participants in your dataset.

## When to Apply

- User interviews for feature decisions
- Churn survey analysis
- NPS/CSAT driver analysis
- Win/loss interview synthesis
- Any qualitative analysis where you have a specific decision to make

Applies equally across **Discover** and **Measure** phases — the technique is identical regardless of when in the lifecycle the research is happening.

## Related

- [Quote Selection Rules for AI Analysis](quote-selection-rules-for-ai-analysis.md) — controls evidence quality
- [Few-Shot Calibration for Analysis Classification](few-shot-calibration-for-analysis.md) — controls classification quality
- [AI Analysis Multi-Pass Verification](ai-analysis-multi-pass-verification.md) — audits the final output

## Sources

**Caitlin Sullivan — "How to Do AI Analysis You Can Actually Trust" (Lenny's Newsletter, 2026-02-18)**
> "Effective context loading has at least four components that shape how AI interprets everything that follows."
> "If outputs are still generic or jumbled after context loading, your context probably wasn't specific enough. Add more detail about what you're actually trying to decide, where your team is trying to go, and what you already know that you don't want repeated."
> "Business goal tells AI what you're trying to achieve. If you need to know whether a feature would attract new users vs. alienate existing ones in order to prioritize building it, say that. AI will weight evidence toward answering your question."

Unique contribution: Naming and structuring the four specific context components; the critical insight that business goal must be framed as a decision with explicit options, not as a research objective.
