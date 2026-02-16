---
title: "Colin Matthews' Workflows for Prototyping with Your Brand's UI"
created: 2026-02-15
updated: 2026-02-15
template: templates/source.md
template_version: 3
tags: [source, ai-pm, claude-added]
status: unread
source_type: podcast
source_url: "https://www.chatprd.ai/how-i-ai/workflows-for-ai-brand-prototyping"
archive_url: ""
author: "Colin Matthews"
host: "Claire Vo"
published: 2025-06-30
discovered: 2026-02-15
summary: "Colin Matthews (PM, founder, Maven instructor) on How I AI. Three workflows for on-brand AI prototyping: (1) Build component library from screenshots in v0 — use a master prompt to create React/Tailwind component library from product screenshots instead of building pages first, iterate by feeding more screenshots, fork the library before building pages so originals stay reusable; (2) Magic Patterns Chrome Extension — click any UI element on a live website to instantly extract and convert it to a clean, reusable React component, build an entire design system in minutes by clicking around your own site; (3) Structured iteration with forks and debugging — use clear naming conventions (Baseline, Var 1, Var 2) for parallel exploration, two-step debugging pattern: diagnose first without writing code, then implement fix. Core insight: improve your building blocks (component primitives) rather than obsessing over tweaking final AI output."
domain: professional-development
project: ai-pm
# taxonomy_inference: product-lifecycle/shape (prototyping-risk-reduction)
# provenance: bulk-added by Claude from podcast-episode-compilation.md (2026-02-15)
# rescrape_needed: false — re-scraped from ChatPRD 2026-02-16
---

# Colin Matthews' Workflows for Prototyping with Your Brand's UI

**By**: Colin Matthews
**Host**: Claire Vo
**Source**: [How I AI (ChatPRD)](https://www.chatprd.ai/how-i-ai/workflows-for-ai-brand-prototyping)
**Type**: podcast

## Summary

How I AI episode with Colin Matthews, PM, founder, and top Maven instructor who has mastered structured AI prototyping. Addresses the core problem: AI tools generate generic, monochrome designs that don't look like your actual product, making it hard to get team buy-in. Three workflows: (1) Build component library from screenshots in v0 — use a detailed master prompt to create React/Tailwind component library from product screenshots instead of building full pages first; iterate by feeding more screenshots from different parts of the app; fork the library before building pages so the original stays as a reusable asset; then assemble pages from pre-approved components; (2) Magic Patterns Chrome Extension — click any UI element on a live website to instantly extract it, AI converts raw HTML/CSS to clean reusable React components; build an entire design system in minutes by clicking around your own site; (3) Structured iteration with forks and debugging — use clear naming conventions (Baseline, Var 1 - Feature, Var 2 - Alternative) for parallel exploration; two-step debugging: "Can you explain why? Don't write any code" then implement fix. Core principle: improve your building blocks (component primitives) rather than obsessing over final output — the assembly becomes more reliable and prototypes reflect the quality of your component library.

## Key Ideas Extracted

- **Components first, pages second**: Build the foundational "Lego bricks" (component library) before generating full pages — this ensures every AI prototype already speaks your brand's visual language
- **Master prompt for component extraction**: Detailed prompt instructs AI to analyze screenshots, identify UI components, create React functional components with Tailwind CSS, and build an index page — sets the standard for the entire project
- **Fork before you build**: Never work directly on your component library; use v0's fork feature to create clean copies for each prototype, preserving the original as a reusable team asset
- **Magic Patterns Chrome Extension**: Click any UI element on a live website to instantly extract and regenerate it as a clean, reusable React component — eliminates need for front-end engineers to pull code
- **Improve primitives, not output**: Focus on making building blocks better rather than obsessing over tweaking final AI output — higher-quality components = more reliable assembly, fewer errors
- **Structured naming for exploration**: Baseline → Var 1 [Feature] → Var 2 [Alternative] — explore multiple creative directions in parallel without losing stable starting points
- **Two-step debugging pattern**: First "explain why, don't write code" to diagnose, then implement fix — forces AI to think before acting, produces much more reliable results
- **AI prototypes as communication tools**: Goal isn't to replace designers/engineers but to give everyone on the team a way to communicate ideas with more detail and clarity

## Notes

- Published Jun 30, 2025 on How I AI (ChatPRD). ~9 min read. (Note: filename says 2025-07-14 but actual publication date is Jun 30, 2025)
- Sponsors: WorkOS, Orkes
- Colin Matthews background: PM, founder, top Maven instructor; runs AI prototyping prompt library
- Tools: v0 (Vercel), Magic Patterns Chrome Extension, React, Tailwind CSS, Next.js
- Demo: Built Airbnb component library and homepage from screenshots
- Three companion workflow guides published Jan 8, 2026
- Cross-references: Prototyping with AI, component-first design systems, structured debugging

## Raw Content

*Re-scraped from ChatPRD 2026-02-16. Full article content captured in Summary and Key Ideas above.*
