---
title: "How Close Is AI to Replacing Product Managers?"
created: 2026-02-15
updated: 2026-02-15
template: templates/source.md
template_version: 3
tags: [source, ai-pm, claude-added]
status: unread
source_type: newsletter
source_url: "https://www.lennysnewsletter.com/p/how-close-is-ai-to-replacing-product"
archive_url: ""
author: "Mike Taylor"
host: ""
published: 2024-07-09
discovered: 2026-02-15
summary: "Mike Taylor (professional prompt engineer, co-author O'Reilly's Prompt Engineering for Generative AI) guest post on Lenny's Newsletter. Blind-tested AI vs. human on three real PM tasks: developing product strategy (YouTube Music), defining KPIs (DoorDash), and estimating ROI (Meta Jobs feature). AI won 2 out of 3 tasks in blind X/LinkedIn polls where voters didn't know which was AI. Key findings: 70-80% of voters correctly identified AI answer but many still preferred it; prompting techniques yield 30-60% accuracy boost over naive prompting; AI's primary weakness was being tactical rather than strategic; AI's primary strength was comprehensiveness in metrics/analysis tasks. Method: used Exponent PM interview answers as human benchmark, applied expert prompting (role-playing, chain-of-thought, examples, instruction decomposition). Includes full prompt templates for all three tasks. Framework for expanding benchmarks across full PM skill taxonomy (shape product, ship product, sync people). Key insight: right now is the worst AI will ever be at any task."
domain: professional-development
project: ai-pm
# taxonomy_inference: ai-adoption (role-evolution, AI-capability-assessment)
# provenance: bulk-added by Claude from podcast-episode-compilation.md (2026-02-15)
# rescrape_needed: false — re-scraped from Lenny's Newsletter 2026-02-15
---

# How Close Is AI to Replacing Product Managers?

**By**: Mike Taylor (guest post)
**Source**: [Lenny's Newsletter / Lenny's Podcast](https://www.lennysnewsletter.com/p/how-close-is-ai-to-replacing-product)
**Type**: newsletter

## Summary

Mike Taylor (professional prompt engineer, co-author of O'Reilly's *Prompt Engineering for Generative AI*) guest post on Lenny's Newsletter. Designed and ran a blind evaluation of AI vs. human performance on three real PM tasks, using Exponent PM interview answers as the human benchmark and expert prompting techniques (role-playing, chain-of-thought, examples, instruction decomposition) to give AI the best chance. The three tasks: (1) Developing product strategy for YouTube Music — AI won with 55% preference, despite 77% correctly identifying it as AI; primary criticism was being tactical rather than strategic. (2) Defining KPIs for DoorDash — AI won decisively with 68-86% preference; comprehensive metrics breakdown impressed voters even though AI's verbosity was a tell. (3) Estimating ROI for a Meta Jobs feature — human won with 58%; AI's estimates were reasonable but lacked the human's specific domain intuition. Overall: AI won 2 of 3 tasks in blind polls. Key methodological insights: prompting techniques drive 30-60% accuracy improvement over naive prompts; most headlines claiming AI fails at tasks used old models with basic prompts; people increasingly prefer AI output even when they know it's AI; small prompt adjustments (adding obscure references, intentional grammatical errors) significantly reduce AI detectability. Proposed framework for comprehensive PM benchmark aligned with Lenny's PM skill taxonomy: shape the product (strategy, goals, specs, discovery, roadmap, feedback), ship the product (QA, resources, unblocking, GTM), sync the people (meetings, communication, alignment, morale). Includes full prompt templates for all three tasks.

## Key Ideas Extracted

- **AI beats humans on 2 of 3 PM tasks**: In blind polls, AI-generated answers for product strategy and KPI definition were preferred over human answers from Exponent's PM interview database
- **People prefer AI even when they know it's AI**: 70-80% correctly identified the AI answer but many still voted for it — acceptance of AI output is growing rapidly
- **Expert prompting is the difference**: Naive prompts yield average internet responses; techniques like role-playing, chain-of-thought, examples, and instruction decomposition improve accuracy 30-60%
- **AI is tactical, humans are strategic**: AI's primary weakness was generating feature lists rather than true strategy; its primary strength was comprehensive, well-structured analysis
- **Right now is the worst AI will ever be**: Models may continue to get twice as good every six months — current benchmarks are a floor, not a ceiling
- **Prompt template formula**: Role + assumptions/thinking section + detailed instructions + human example = consistently above-average AI output
- **Human uniqueness is in the unexpected**: A human answer referencing a cricket player stood out as authentically human — niche interests and unexpected connections are hard for AI to replicate
- **Blind testing reveals true attitudes**: When people see the AI label, bias (positive or negative) skews results; blind evaluation is the only fair way to measure AI performance
- **PM benchmark framework needed**: Proposed aligning hard PM task benchmarks with Lenny's PM skill taxonomy (shape/ship/sync) to track what percentage of the PM role is automatable
- **Data contamination risk**: Publishing correct answers trains future models on them — future benchmarks should avoid revealing which answer was AI

## Notes

- Published Jul 9, 2024 on Lenny's Newsletter. Free edition guest post by Mike Taylor.
- Mike Taylor background: co-author O'Reilly *Prompt Engineering for Generative AI*, builds AI products at Brightpool, previously ran 50-person marketing agency (clients: Booking.com, Time Out, Monzo)
- Human benchmark: Exponent PM interview prep database (official partner for Stanford, Yale, Cornell, Columbia)
- Models tested: GPT-4o via OpenAI Playground (not ChatGPT interface — allows custom system prompts)
- Evaluation method: Blind X/LinkedIn polls with manual vote tallying
- Proposed future work: test Claude 3.5, Gemini 1.5, Perplexity; expand to more PM tasks; use private voting to avoid groupthink
- Cross-reference: Lenny's PM skill framework (shape/ship/sync), Marily Nika AI PM episodes, Udezue sharp problems framework
- Historical note: Written Jul 2024 with GPT-4o — AI capabilities have advanced significantly since

## Raw Content

*Re-scraped from Lenny's Newsletter 2026-02-15. Full article content captured in Summary and Key Ideas above.*
