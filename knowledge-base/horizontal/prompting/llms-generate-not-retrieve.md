---
created: 2026-02-18
updated: 2026-02-18
tags: [knowledge, ai-pm]
status: draft
origin: sourced
featured: false
entry_type: mental-model
domain: horizontal
horizontal_domain: prompting
---

# LLMs Generate, Not Retrieve

LLMs produce text by generating statistically plausible continuations given the context — they do not search for and return existing text. This distinction explains why AI confidently produces wrong answers, fabricated quotes, and invented citations.

## The Model

When you ask an AI to "find" something in a source — a quote, a statistic, a specific claim — the model doesn't scan the text and pull a match. It generates text that is statistically likely to be what you're looking for, given the context you've provided and its training data. If the context is about pricing concerns, it will produce plausible-sounding pricing language. If asked for a verbatim quote from a user interview, it generates what a quote *should* sound like.

This is why:
- **Hallucinated quotes look real** — the model knows what user research quotes sound like; it generates from that pattern
- **Citations look authoritative** — "[P03, 14:30]" is plausible formatting for a citation, so the model produces it whether or not P03 said anything at 14:30
- **Errors look confident** — the model's confidence reflects how statistically likely its output is, not how accurate it is
- **AI analysis gives consistent-looking results from sparse data** — it can produce a clean 5-theme synthesis from 2 interviews, because themes are generated from training priors, not retrieved from the data

## Why This Is a Foundational Mental Model

Most prompting failures and evaluation failures trace back to treating AI output as *retrieval* when it's actually *generation*. Understanding this model immediately clarifies:
- Why you need quote verification (retrieved → verified vs. generated → must check)
- Why specificity in prompts matters (generation fills in ambiguous gaps with plausible defaults)
- Why AI analysis output always looks confident (generation confidence ≠ factual accuracy)
- Why "just ask the AI to be more careful" doesn't fix hallucinations (it changes the generation pattern, not the underlying mechanism)

## Implications for PM Workflows

- **User research**: Always verify AI-extracted quotes before attributing to participants
- **Competitive analysis**: AI-generated market stats and competitor claims require source verification
- **PRD drafts**: AI-generated requirements may sound specific and grounded but be generated from patterns, not facts
- **Summaries of long documents**: AI summarizes by generating likely-sounding abstractions, not by faithfully compressing content

## Related

- [Quote Selection Rules for AI Analysis](../../product-lifecycle/discover/quote-selection-rules-for-ai-analysis.md) — practical application to qualitative research
- [Quote Verification Pass](../../product-lifecycle/discover/quote-verification-pass.md) — the verification technique that corrects for this
- [AI Analysis Multi-Pass Verification](../../product-lifecycle/discover/ai-analysis-multi-pass-verification.md) — full verification framework

## Sources

**Caitlin Sullivan — "How to Do AI Analysis You Can Actually Trust" (Lenny's Newsletter, 2026-02-18)**
> "LLMs don't retrieve quotes like a search engine; they generate text that's statistically likely given the context. Generation and retrieval are fundamentally different. The model predicts what a quote should look like."
> "Even participant IDs and timestamps can be faked. A citation like '[P03, 14:30]' looks authoritative but means nothing if the quote is invented."

Unique contribution: Naming the generation vs. retrieval distinction explicitly as the root cause of AI analysis failure modes; showing how this one model explains all four failure modes.
