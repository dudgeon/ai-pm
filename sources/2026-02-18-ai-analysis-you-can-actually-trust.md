---
title: "How to Do AI Analysis You Can Actually Trust"
created: 2026-02-18
updated: 2026-02-18
processed: 2026-02-18
template: templates/source.md
template_version: 3
tags: [source, ai-pm]
status: processed
source_type: newsletter
source_url: "https://www.lennysnewsletter.com/p/how-to-do-ai-analysis-you-can-actually"
archive_url: ""
author: "Caitlin Sullivan"
host: "Lenny Rachitsky"
published: 2026-02-18
discovered: 2026-02-18
summary: "Four systematic failure modes of AI-assisted qualitative analysis — invented evidence, false/generic insights, non-decision-guiding signal, contradictory insights — each with prompt-level fixes: quote selection rules + verification pass, decision-anchored context loading (4 components), few-shot calibration with labeled examples, multi-pass contradiction audit. Includes comparative model guidance: Claude for depth/breadth, Gemini for evidenced themes, ChatGPT for stakeholder framing. Root cause of most failures: LLMs generate statistically plausible text, they don't retrieve it."
domain: professional-development
project: ai-pm
---

# How to Do AI Analysis You Can Actually Trust

**By**: Caitlin Sullivan (guest in Lenny's Newsletter)
**Source**: [Lenny's Newsletter](https://www.lennysnewsletter.com/p/how-to-do-ai-analysis-you-can-actually)
**Type**: newsletter

## Summary

AI analysis output always looks confident — clean themes, punchy quotes, tidy summaries — even when full of errors. Caitlin Sullivan identifies four systematic failure modes of AI-assisted qualitative analysis (interviews, surveys) and provides prompt-level fixes for each. The root cause threading through all four: LLMs generate statistically plausible text rather than retrieving it, so they will always produce something that looks right unless you design checks to catch errors.

## Key Ideas Extracted

- [Quote Selection Rules for AI Analysis](../knowledge-base/product-lifecycle/discover/quote-selection-rules-for-ai-analysis.md) — Define exact quote rules before extraction to prevent AI from generating plausible-sounding paraphrases `discover/problem-signal-detection`
- [Quote Verification Pass](../knowledge-base/product-lifecycle/discover/quote-verification-pass.md) — Dedicated follow-up prompt to confirm each extracted quote is verbatim in the source `discover/problem-signal-detection`
- [Decision-Anchored Analysis Context](../knowledge-base/product-lifecycle/discover/decision-anchored-analysis-context.md) — Load 4 context components (project context, business goal, product context, participant overview) to anchor AI analysis to your specific decision `discover/problem-signal-detection`
- [Few-Shot Calibration for Analysis Classification](../knowledge-base/product-lifecycle/discover/few-shot-calibration-for-analysis.md) — Give AI labeled examples with rationale for each category level to prevent invented classification criteria `discover/problem-signal-detection`
- [AI Analysis Multi-Pass Verification](../knowledge-base/product-lifecycle/discover/ai-analysis-multi-pass-verification.md) — Deliberate second pass targeting quote errors, within-participant contradictions, and thin evidence `discover/problem-signal-detection`
- [LLMs Generate, Not Retrieve](../knowledge-base/horizontal/prompting/llms-generate-not-retrieve.md) — Root cause mental model: LLMs produce statistically plausible text, not retrieved text `horizontal/prompting`
- [Model Fit for Qualitative Analysis Tasks](../knowledge-base/horizontal/agents/managing-agents/selection/model-fit-for-qualitative-analysis.md) — Claude (depth/breadth), Gemini (evidence), ChatGPT (framing) as distinct use cases `horizontal/agents/managing-agents/selection`

## Notes

- Sullivan's framing of "four failure modes" is a useful pedagogical structure for teaching AI analysis to PMs
- The WHOOP screen decision serves as a single running example throughout — good for grounding abstract techniques
- Model comparison section (Claude vs Gemini vs ChatGPT for analysis) is empirically grounded (2,000+ hours of testing) but will get stale as models evolve. Capture the *framework* (depth vs. evidence vs. communication) more than the specific rankings
- The "few-shot calibration" technique extends directly beyond analysis — applicable anywhere you want AI to apply consistent classification criteria (user segmentation, feedback tagging, priority scoring, etc.)
- The survey column disambiguation guidance is underappreciated: "Data Structure vs. Analysis Quality Gap" — AI treats every column as signal unless told otherwise
- The generation vs. retrieval distinction is the foundational mental model that explains all four failure modes

## Raw Content

### Four Failure Modes of AI Analysis

**Failure Mode 1: Invented Evidence**

LLMs don't retrieve quotes like a search engine; they generate text that's statistically likely given the context. "Verbatim" is ambiguous — the model predicts what a quote *should* look like. Prompting for "punchy, max 12-word quotes" triggers synthesis.

Fix — **Quote Selection Rules**:
- Start where the thought begins, continue until fully expressed
- Include reasoning, not just conclusions
- Keep hedges and qualifiers — they signal uncertainty
- Include emotional language when present
- Cite with participant ID and approximate timestamp `[P02 ~14:30]`
- Do not combine statements from different parts of the interview
- If a quote would exceed 3 sentences, break into separate quotes

Fix — **Quote Verification Pass** (run after initial analysis):
> For each quote: (1) Confirm verbatim in source, (2) If paraphrase, flag and give actual wording, (3) If not found, mark NOT FOUND. Output: Status = VERIFIED / PARAPHRASE / NOT FOUND + Location.

**Failure Mode 2: False or Generic Insights**

AI defaults to consensus patterns. It misses edge cases that matter, creates themes that "could describe any product in your category," and gets primed by terms you accidentally include in the prompt.

Fix — **Decision-Anchored Context Loading** (4 components):
1. **Project context**: Scope and stakes ("Exploring whether to add a screen — major hardware decision, 10 churned user interviews")
2. **Business goal**: The specific decision, not just the objective ("Determine if screen would win back churned users, fail to solve their core problems, or require other changes")
3. **Product context**: Domain knowledge — what the product is, what competitors do, the core tension being explored
4. **Participant overview**: Who's speaking, their relationship to the product, what segment they represent

Survey-specific: Also provide data structure (which columns are customer voice vs. metadata) and interpretation guidance (e.g., "0 = churned, 1 = active").

**Failure Mode 3: Signal That Doesn't Guide Decisions**

Counts without decision clarity. "22 people mentioned screens" doesn't tell you whether building a screen would retain them, or whether they'd actually need other features too.

Fix — **Few-Shot Calibration**:
Define a solution-fit scale with concrete examples of each level — not descriptions of what levels *mean* but actual examples of responses that belong there, *and why*. The examples do the teaching; they remove ambiguity that lets AI fill gaps with its own interpretation.

Example: A 5-level "Would a screen retain this user?" scale, with examples:
- Level 1 (screen would retain): "I check my phone 10 times per workout just to see my HR" — explains *why* this is a 1: specific friction, screen directly solves it
- Level 5 (unrelated competitive loss): "Switched to Apple Watch, Whoop was fine" — explains *why*: no negative language, screen irrelevant

**Failure Mode 4: Contradictory Insights**

AI presents everything with equal confidence. It doesn't flag when a participant contradicted themselves at minute 8 vs. minute 35. The first pass is always a hypothesis; without a second review pass, you're treating a draft as final.

Fix — **Multi-Pass Verification Prompt**:
> Review the analysis above for: (1) Quote verification — confirm verbatim in source, flag paraphrases/not found; (2) Contradiction check — for each participant, check if statements conflict (stated preferences vs. behaviors, confidence followed by hedging, strong opinions that soften); (3) Confidence assessment — flag findings based on limited evidence, note unclear/mixed stances. Output: Verification summary with flags and recommended revisions.

### Model Comparison for Analysis Work

Based on 2,000+ hours of testing:

| Model | Strength | Tradeoff |
|---|---|---|
| **Claude** | Depth + breadth; covers most ground, stays data-grounded | Doesn't filter — validated patterns and half-formed hypotheses presented equally; you do the filtering |
| **Gemini** | Fewer themes but strongly evidenced; best for video analysis | Requires multiple prompts to get completeness; chooses short quote snippets |
| **ChatGPT** | Best for framing and stakeholder communication | Most creative — including with "verbatim quotes"; least reliable evidence (combines quotes) |

Recommendation: Claude for analysis work. Tradeoff is manageable: you get breadth without having to push for it, and you verify themes rather than prompt repeatedly.
