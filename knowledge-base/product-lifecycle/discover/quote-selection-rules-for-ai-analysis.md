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

# Quote Selection Rules for AI Analysis

When prompting AI to extract quotes from qualitative research data (interview transcripts, survey responses), define explicit quote rules before the extraction request. Without this, AI generates statistically plausible text that *sounds* like what the participant said — not necessarily what they actually said.

## The Technique

Add a `QUOTE SELECTION RULES` block to any analysis prompt before requesting themes or evidence:

```
QUOTE SELECTION RULES
• Start where the thought begins, and continue until fully expressed
• Include reasoning, not just conclusions
• Keep hedges and qualifiers — they signal uncertainty
• Include emotional language when present
• Cite with participant ID and approximate timestamp [P02 ~14:30]
• Do not combine statements from different parts of the interview
• If a quote would exceed 3 sentences, break into separate quotes
```

## Why It Works

LLMs don't retrieve quotes — they generate text that is statistically plausible given the context. "Verbatim" means nothing without a definition. The model predicts what a quote *should* look like, filling in gaps with training data about how people typically express similar sentiments. Quote rules remove this ambiguity by specifying exactly where to start, where to stop, what to include, and what not to combine.

Prompts that trigger synthesis: "Give me a punchy representative quote (max 12 words)" or "summarize in the customer's voice." These are instructions to synthesize, not retrieve.

## When to Apply

- Extracting themes from interview transcripts
- Coding survey open-response fields
- Building evidence sections for research readouts
- Any context where specific participant language will be used as evidence

Also applies equally to **Measure** phase work: customer feedback collection, NPS/CSAT analysis, support theme identification.

## Related

- [Quote Verification Pass](quote-verification-pass.md) — the follow-up check that confirms extracted quotes are real
- [Decision-Anchored Analysis Context](decision-anchored-analysis-context.md) — sets up the full analysis frame before extraction
- [LLMs Generate, Not Retrieve](../../horizontal/prompting/llms-generate-not-retrieve.md) — the root cause mental model

## Sources

**Caitlin Sullivan — "How to Do AI Analysis You Can Actually Trust" (Lenny's Newsletter, 2026-02-18)**
> "LLMs don't retrieve quotes like a search engine; they generate text that's statistically likely given the context. Generation and retrieval are fundamentally different."
> "Even participant IDs and timestamps can be faked. A citation like '[P03, 14:30]' looks authoritative but means nothing if the quote is invented."

Unique contribution: Framing of the generation vs. retrieval root cause; concrete quote rules prompt template tested across 2,000+ hours of analysis work.
