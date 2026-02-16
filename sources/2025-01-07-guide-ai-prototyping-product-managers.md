---
title: "A Guide to AI Prototyping for Product Managers"
created: 2026-02-15
updated: 2026-02-15
template: templates/source.md
template_version: 3
tags: [source, ai-pm, claude-added]
status: unread
source_type: newsletter
source_url: "https://www.lennysnewsletter.com/p/a-guide-to-ai-prototyping-for-product"
archive_url: ""
author: "Colin Matthews"
host: ""
published: 2025-01-07
discovered: 2026-02-15
summary: "Colin Matthews (PM @ Datavant, AI prototyping course instructor) guest post on Lenny's Newsletter. Comprehensive guide to AI prototyping tools organized into three categories: chatbots (Claude, ChatGPT — best for single-page prototypes), cloud development environments (v0, Bolt, Replit, Lovable — best for multi-feature prototypes), and local developer assistants (Cursor, GitHub Copilot, Windsurf, Zed — best for production apps). Tool selection guide: v0 for beautiful designs by default, Bolt for quick prototypes with flexible designs, Replit for internal/data-driven tools, Lovable for production apps with integrations. Six prompt templates for common use cases: Figma-to-prototype, scratch builds, data dashboards, hand-drawn mockup conversion, PRD-to-prototype, and personal productivity tools. Four debugging strategies for non-coders: reflection (force AI to plan before coding), batching (small incremental changes), being specific (detailed instructions), and managing lost context (checkpoints and focused changes). End-to-end walkthrough building Airbnb price filter prototype in under 10 minutes."
domain: professional-development
project: ai-pm
# taxonomy_inference: product-lifecycle/shape (prototyping-risk-reduction); software-methodology (vibe-coding, tool-landscape)
# provenance: bulk-added by Claude from podcast-episode-compilation.md (2026-02-15)
# rescrape_needed: false — re-scraped from Lenny's Newsletter 2026-02-15
---

# A Guide to AI Prototyping for Product Managers

**By**: Colin Matthews
**Source**: [Lenny's Newsletter / Lenny's Podcast](https://www.lennysnewsletter.com/p/a-guide-to-ai-prototyping-for-product)
**Type**: newsletter

## Summary

Colin Matthews guest post on Lenny's Newsletter — a comprehensive guide to AI prototyping for product managers. Organizes the AI development tool landscape into three categories: (1) **Chatbots** (Claude, ChatGPT) — best for single-page prototypes like calculators or data visualizations; Claude's Artifacts can deploy to shareable links but lack direct code editing. (2) **Cloud development environments** (v0, Bolt, Replit, Lovable) — the sweet spot for PMs; handle building, hosting, and deploying multi-feature apps. v0 excels at beautiful defaults using Next.js/Shadcn UI; Bolt is fast for flexible prototypes but runs server code in-browser (no auth/persistence); Replit provides full-stack with database, great for internal tools and Python; Lovable best for production apps with GitHub/Supabase/AI integrations but lacks code editor. (3) **Local developer assistants** (Cursor, GitHub Copilot, Windsurf, Zed) — for people who know code, working on production apps. Includes end-to-end walkthrough building an Airbnb price filter prototype in under 10 minutes using Bolt, converting a Figma screenshot to working app with three iterative prompts. Six prompt templates cover common PM use cases: Figma-to-prototype, scratch builds with good UI defaults, data dashboards, hand-drawn mockup conversion, PRD-to-prototype, and personal productivity tools. Four debugging strategies for non-coders: reflection (force AI to plan before coding), batching (build smallest functional increment first, start with data model), being specific (describe changes in detail like working with a junior engineer), and managing lost context (use checkpoints, focus AI on specific files).

## Key Ideas Extracted

- **Three-tier tool taxonomy**: Chatbots (simple, one-page) → Cloud dev environments (multi-feature, deployed) → Local IDEs (production, code-proficient) — choose tier based on complexity and coding ability
- **Tool selection framework**: v0 for beautiful designs, Bolt for quick flexible prototypes, Replit for internal/data tools, Lovable for production with integrations — each has distinct strengths
- **Figma-to-prototype in minutes**: Screenshot a Figma design, paste into Bolt with "match this exactly," then iterate with specific prompts — eliminates weeks of engineering wait time
- **Reflection as debugging strategy**: Force AI to plan before coding by explicitly saying "do not write any code, only explain" — produces better results and helps non-coders understand what's happening
- **Batching beats front-loading context**: Build the smallest functional increment first rather than describing everything upfront — counterintuitive but more effective; start with data model as backbone
- **Specificity as prompting superpower**: Describe changes like you're working with a junior engineer — what technologies, what parts of the product, what files, even what lines of code should change
- **Lost context prevention**: AI tools rewrite entire sections when instructions are vague — use checkpoints to roll back, combine reflection + batching + specificity to minimize destructive rewrites
- **PRD-to-prototype workflow**: Copy-paste PRD into Bolt with screenshots and "follow exact specifications" — turns specification documents directly into interactive prototypes
- **Cloud environments as PM sweet spot**: Cloud dev environments handle the full stack (client, server, database, hosting) that chatbots can't — the right abstraction level for PM prototyping

## Notes

- Published Jan 7, 2025 on Lenny's Newsletter. Subscriber-only guest post by Colin Matthews.
- Colin Matthews background: PM @ Datavant, first SaaS product acquired 2021, teaches AI Prototyping for Product Managers course on Maven (4-week cohort), 5000+ students
- Also wrote Lenny's 9th most popular post of all time ("Become a more technical product manager")
- Tools covered: Claude, ChatGPT, Perplexity, v0, Bolt, Replit, Lovable, Cursor, GitHub Copilot, Windsurf, Zed
- Frameworks/libraries mentioned: Next.js, Shadcn UI, Tailwind CSS, Supabase, React, Streamlit, Python, Node.js
- Cross-reference: Part 2 is `2025-06-10-get-entire-team-prototyping-ai.md` (same author, team-level adoption)
- This is Part 1 — foundational tool landscape and individual PM techniques; Part 2 covers organizational adoption

## Raw Content

*Re-scraped from Lenny's Newsletter 2026-02-15. Full article content captured in Summary and Key Ideas above.*
