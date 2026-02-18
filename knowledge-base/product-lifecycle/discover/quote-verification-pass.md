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

# Quote Verification Pass

After AI extracts themes and supporting quotes from qualitative data, run a dedicated verification prompt asking the AI to confirm each quote exists verbatim in the source. This is a separate pass, not part of the initial extraction — AI produces more accurate verifications when explicitly auditing its own work.

## The Technique

After the initial analysis, send this follow-up prompt:

```
QUOTE VERIFICATION

For each quote in the analysis above:
1. Confirm the quote exists verbatim in the source transcript
2. If the quote is a close paraphrase but not exact, flag it and provide the actual wording
3. If the quote cannot be located, mark as NOT FOUND

Output format:
• Quote: [the quote]
• Status: VERIFIED / PARAPHRASE / NOT FOUND
• If paraphrase: Actual wording: [what they said]
• Location: [Participant ID, timestamp, or line number]
```

## What It Catches

- **Paraphrases** — AI combined the gist of what someone said with statistically likely phrasing; the meaning may be close but the words aren't theirs
- **Frankenstein quotes** — statements sewn together from multiple moments in the interview; looks authentic, isn't
- **Fabricated citations** — timestamps and participant IDs that look authoritative but reference passages that don't exist
- **Confident-sounding errors** — AI presents all quotes with equal confidence; verification reveals which are solid

When run on ChatGPT-generated quotes, this frequently reveals that a majority of quotes are paraphrased rather than verbatim, even when the extraction prompt explicitly asked for verbatim quotes.

## When to Apply

- Before any research readout where quotes will be attributed to specific participants
- Whenever the initial extraction asked for short/punchy quotes (high synthesis risk)
- For any analysis where specific wording matters (messaging validation, pricing research, emotional resonance)

Also applies to **Measure** phase: customer feedback analysis, churn interview synthesis, NPS driver analysis.

## Notes

- This adds ~5 minutes to analysis workflow
- Running AI as a self-auditor works better than expecting it to catch errors in the initial pass — verification is a cognitively different task than extraction
- If source transcripts are very long, specify which section of the transcript to search in the verification prompt

## Related

- [Quote Selection Rules for AI Analysis](quote-selection-rules-for-ai-analysis.md) — the upstream technique that reduces errors before they happen
- [Multi-Pass AI Analysis Verification](ai-analysis-multi-pass-verification.md) — the broader verification framework that includes this as one component
- [LLMs Generate, Not Retrieve](../../horizontal/prompting/llms-generate-not-retrieve.md) — root cause mental model

## Sources

**Caitlin Sullivan — "How to Do AI Analysis You Can Actually Trust" (Lenny's Newsletter, 2026-02-18)**
> "A majority of the quotes in the previous ChatGPT output were paraphrased, not original verbatim customer statements. This happened with a request for a small set of quotes, so imagine what happens when you're digging through 20 interviews."
> "Without verification, 'quotes' like these end up in your deck attributed to a real participant. Sometimes it's no big deal. Other times, it's the difference between product language that strongly resonates and messaging that doesn't convert."

Unique contribution: Specific verification prompt template; empirical finding that verification frequently uncovers paraphrases even when verbatim was requested.
