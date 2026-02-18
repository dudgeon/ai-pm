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

# AI Analysis Multi-Pass Verification

AI analysis is always a first draft — it finds patterns, extracts quotes, and builds themes, all presented with equal confidence. Without a deliberate second pass targeting specific failure modes, errors stay invisible until a stakeholder asks a question you can't answer or a decision fails three months later.

## The Technique

After completing initial AI analysis, run a verification pass that explicitly targets three error types:

```
VERIFICATION PASS

Review the analysis above for:

1. QUOTE VERIFICATION
   • Confirm each quote exists verbatim in the source
   • Flag any quotes that are paraphrased, combined, or not found

2. CONTRADICTION CHECK
   • For each participant, check if statements at different points conflict
   • Look for: stated preferences vs. described behaviors, confidence
     followed by hedging, strong opinions that soften later in the interview

3. CONFIDENCE ASSESSMENT
   • For any finding based on limited evidence, flag it
   • Note participants where the stance is unclear or mixed

Output a verification summary with flags and recommended revisions.
```

## Why a Separate Pass Is Necessary

AI is trained to produce coherent, helpful responses — not to flag its own uncertainty. The first pass is an extraction-and-synthesis task; the verification pass is an auditing task. These are cognitively different enough that AI performs better when they're separated.

Expert human analysts do multiple passes instinctively. AI doesn't, unless prompted. Running the verification prompt causes the AI to find errors it didn't flag in the initial analysis — sometimes significant ones (wrong classifications, missed contradictions, thin evidence presented as strong themes).

## The Three Error Types This Catches

**Quote errors** — Paraphrased, synthesized, or fabricated quotes presented as verbatim participant language. (→ see [Quote Verification Pass](quote-verification-pass.md) for the dedicated quote check prompt)

**Within-participant contradictions** — A participant who says "I love the data tracking" at minute 8 but "I stopped checking it after two weeks" at minute 35. AI's initial synthesis may collapse this into a positive sentiment theme.

**Thin evidence** — Themes built on one or two data points, presented with the same confidence as themes built on eight. "Pricing is a concern" based on one throwaway comment vs. a consistent thread across the full dataset.

## Notes

- This pass adds 5–10 minutes to analysis but prevents costly errors in downstream decisions
- Verification is faster and more accurate if source transcripts are organized by participant (AI can more easily check contradictions within a participant's transcript)
- The verification prompt can be run multiple times if the first verification reveals significant issues that require re-analysis
- This is the final check; run it after all other techniques (context loading, calibration, extraction) are in place

## Related

- [Quote Selection Rules for AI Analysis](quote-selection-rules-for-ai-analysis.md) — reduce errors before extraction
- [Quote Verification Pass](quote-verification-pass.md) — focused version for quote fidelity alone
- [Decision-Anchored Analysis Context](decision-anchored-analysis-context.md) — reduces generic insights (Failure Mode 2)
- [Few-Shot Calibration for Analysis Classification](few-shot-calibration-for-analysis.md) — reduces non-decision-guiding signal (Failure Mode 3)

## Sources

**Caitlin Sullivan — "How to Do AI Analysis You Can Actually Trust" (Lenny's Newsletter, 2026-02-18)**
> "Most people skip contradiction verification because stories in the first analysis pass feel complete. AI doesn't say, 'By the way, I'm not sure about Participant 03.' It presents everything with equal confidence."
> "Human expert analysts do multiple passes instinctively. AI doesn't, unless you tell it to. That's by design. LLMs are trained to produce coherent, helpful responses, not to flag their own uncertainty, by default."
> "When you push any LLM to review its own labeling and interpretation, it actually will find errors."
> "Verification is the difference between AI output you'll always second-guess and insights you can stand behind."

Unique contribution: The "separate pass as different cognitive task" framing; the three-part verification framework targeting quotes + contradictions + confidence; empirical finding that AI finds errors when explicitly asked to audit its own work.
