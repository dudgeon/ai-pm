---
title: "Hamel Husain's Guide to Debugging AI Products and Writing Evals"
created: 2026-02-15
updated: 2026-02-15
template: templates/source.md
template_version: 3
tags: [source, ai-pm, claude-added]
status: unread
source_type: podcast
source_url: "https://www.chatprd.ai/how-i-ai/debugging-ai-writing-evals"
archive_url: ""
author: "Hamel Husain"
host: "Claire Vo"
published: 2025-08-04
discovered: 2026-02-15
summary: "AI consultant Hamel Husain presents a 6-step systematic error analysis framework for debugging AI products: log traces → manual error analysis → custom annotation → frequency-based prioritization → targeted evals (code-based + LLM judges) → iterate with prompt engineering or fine-tuning. Also demonstrates running entire consulting business via Claude Projects and a GitHub monorepo as centralized 'second brain' for AI context."
domain: professional-development
project: ai-pm
# taxonomy_inference: product-lifecycle/measure (experiment-design-analysis); horizontal/agents (agent-quality); horizontal/context (mono-repo-as-context)
# provenance: bulk-added by Claude from podcast-episode-compilation.md (2026-02-15)
# rescrape_needed: false — re-scraped from ChatPRD 2026-02-15
---

# Hamel Husain's Guide to Debugging AI Products and Writing Evals

**By**: Hamel Husain
**Host**: Claire Vo
**Source**: [How I AI (ChatPRD / Lenny's Podcast Network)](https://www.chatprd.ai/how-i-ai/debugging-ai-writing-evals)
**Type**: podcast

## Summary

Two distinct workflows presented. **Workflow 1** is a 6-step systematic error analysis framework for AI products: (1) log and examine real user traces, (2) perform manual error analysis via "open coding" on ~100 sampled traces, (3) build custom annotation systems to speed up review, (4) categorize and prioritize errors by simple frequency counting, (5) write targeted evals using code-based checks for deterministic issues and LLM judges for subjective ones, (6) iterate with prompt engineering or fine-tuning. **Workflow 2** covers Hamel's personal AI-powered business operations: Claude Projects as dedicated spaces for each business function (copywriting, proposals, courses), Gemini for multimodal content transformation (video → annotated presentations), and a GitHub monorepo as a centralized "second brain" providing context to all AI tools.

## Key Ideas Extracted

- **Traces over test cases**: Real user interaction traces (full multi-turn conversations including tool calls, RAG lookups, system prompts) reveal the true distribution of inputs — synthetic data can't substitute
- **First-error heuristic**: When reviewing traces, stop at the first error in the sequence — fixing upstream intent clarification or tool call issues often resolves downstream failures
- **Frequency counting as prioritization**: Simple counting of categorized error notes produces a data-driven roadmap; moves teams past analysis paralysis
- **Binary LLM judges with human validation**: LLM-as-judge evals should produce binary pass/fail (not arbitrary scores like 4.2 vs 4.7). Must validate against hand-labeled data to measure agreement — skipping this creates false confidence
- **Two flavors of evals**: Code-based evals for deterministic checks (e.g., sensitive data not leaking into responses), LLM judges for nuanced/subjective issues
- **Claude Projects as business function spaces**: Separate project for each function (proposals, legal, courses) pre-loaded with style guides, examples, and context
- **GitHub monorepo as AI second brain**: Single private repo holding all data sources, notes, prompts, and tools — provides complete context to AI co-pilots and prevents vendor lock-in
- **Gemini for video-to-text transformation**: Multimodal processing to create annotated presentations from YouTube videos, with slide screenshots + transcript summaries

## Notes

- Published on ChatPRD blog Oct 14, 2025 (episode aired ~Aug 4, 2025). 11-min read.
- References the research paper "Who Validates the Validators?" on aligning LLM evaluation with human preferences
- Demo used Nurture Boss (AI assistant for property managers) as the example product
- Tools mentioned: Braintrust, Arize (trace logging/observability), Claude Projects, Gemini, GitHub monorepo, Cursor, Claude Code
- The monorepo approach echoes patterns from other episodes (Ryan Carson's three-file system, Teresa Torres's context libraries)
- Transition matrices mentioned as advanced technique for agent-based systems with multiple handoffs

## Raw Content

*Re-scraped from ChatPRD 2026-02-15. Full article content captured in Summary and Key Ideas above.*
