---
title: "Data-Driven Prototyping and Structured Midjourney Prompts for Elite Results"
created: 2026-02-15
updated: 2026-02-15
template: templates/source.md
template_version: 3
tags: [source, ai-pm, claude-added]
status: unread
source_type: podcast
source_url: "https://www.chatprd.ai/how-i-ai/data-driven-prototyping-and-structured-midjourney-prompts"
archive_url: ""
author: "Ravi Mehta"
host: "Claire Vo"
published: 2025-09-29
discovered: 2026-02-15
summary: "Ravi Mehta (fmr CPO, Tinder) presents two workflows: (1) Data-driven prototyping — generate structured JSON data models with Claude (+ Unsplash MCP for real media) BEFORE building UI, applying separation of concerns so the AI focuses on UX rather than juggling data/code/design simultaneously. Uses Reforge Build for prototyping. (2) Subject-Setting-Style framework for Midjourney — use photographic vocabulary (film stocks like Kodak Trix, camera metadata like Leica 50mm F1.2) to guide image generation toward higher-quality training data. Argues art literacy is becoming a core AI skill."
domain: professional-development
project: ai-pm
# taxonomy_inference: product-lifecycle/shape (prototyping-risk-reduction); horizontal/prompting (structured-prompting)
# provenance: bulk-added by Claude from podcast-episode-compilation.md (2026-02-15)
# rescrape_needed: false — re-scraped from ChatPRD 2026-02-15
---

# Data-Driven Prototyping and Structured Midjourney Prompts for Elite Results

**By**: Ravi Mehta
**Host**: Claire Vo
**Source**: [How I AI (ChatPRD / Lenny's Podcast Network)](https://www.chatprd.ai/how-i-ai/data-driven-prototyping-and-structured-midjourney-prompts)
**Type**: podcast

## Summary

Two workflows addressing the "vibe prototyping" problem — asking AI to simultaneously handle UX, code architecture, and data structure produces mediocre results. **Workflow 1 (Data-Driven Prototyping)**: Generate structured JSON data with Claude first, using Unsplash MCP server for real image URLs, then feed that JSON to a prototyping tool (Reforge Build) with a minimal prompt. Separation of concerns lets the AI focus purely on optimal UX for the given data. Enables easy iteration: swap JSON for different destinations/languages, stress-test with edge-case content lengths, augment existing data without starting over. **Workflow 2 (Structured Midjourney Prompting)**: Subject-Setting-Style framework — define what you're showing, where/lighting, and how it should look using photographic vocabulary. Film stocks (Kodak Trix, Fuji Color C200, Fujifilm Provia) and camera metadata (Leica, 50mm, F1.2) steer the model toward higher-quality aesthetic regions of its training data.

## Key Ideas Extracted

- **Separation of concerns in prototyping**: Don't ask AI to solve UX, data schema, and code architecture simultaneously — generate structured data first, then let the prototyping tool focus solely on UI/UX
- **MCP servers for real media**: Unsplash MCP in Claude provides actual image URLs, eliminating hallucinated/broken images that plague vibe prototyping
- **JSON-first prototyping enables iteration**: Swap datasets for different scenarios (destinations, languages, content lengths) without rebuilding the prototype; stress-test edge cases in design reviews
- **Subject-Setting-Style framework for Midjourney**: Three-element prompt structure that produces professional-quality images vs. generic "vibe prompt" results
- **Film stock + camera metadata as "cheat code"**: Specific photographic references (Kodak Trix for B&W contrast, Leica for premium aesthetics, F1.2 for bokeh) point the model toward higher-quality training data regions
- **Art literacy as AI skill**: Understanding visual vocabulary (lighting, composition, style references) directly improves prompt quality — recommend using Claude/ChatGPT to describe photos you like to build this vocabulary
- **"Elite" keyword for quality guidance**: Adding qualifiers like "elite" to prompts guides AI toward higher-quality training data associations
- **AI enables "nice-to-have" features**: Personalization and delight features that get cut from scope become feasible with AI — competitive advantage for consumer products

## Notes

- Published Sep 28, 2025 on ChatPRD blog. 10-min read.
- Tools: Claude (JSON generation), Unsplash MCP server, Reforge Build (prototyping), Midjourney (image generation)
- Ravi also has an AI Strategy course with Brian Balfour through Reforge
- Practical detail: Claude generates JSON with real Unsplash URLs via MCP calls, but this takes extra time due to multiple API calls
- The data-driven approach produces clean, componentized code where data lives in lib/sampleData.ts for easy swapping
- Sponsors: Google Gemini, Persona

## Raw Content

*Re-scraped from ChatPRD 2026-02-15. Full article content captured in Summary and Key Ideas above.*
