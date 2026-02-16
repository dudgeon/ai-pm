---
title: "How to Get Your Entire Team Prototyping with AI"
created: 2026-02-15
updated: 2026-02-15
template: templates/source.md
template_version: 3
tags: [source, ai-pm, claude-added]
status: unread
source_type: newsletter
source_url: "https://www.lennysnewsletter.com/p/how-to-get-your-entire-team-prototyping"
archive_url: ""
author: "Colin Matthews"
host: "Lenny Rachitsky"
published: 2025-06-10
discovered: 2026-02-15
summary: "Colin Matthews (guest post on Lenny's Newsletter) presents a comprehensive guide to scaling AI prototyping across product teams. Three approaches to component libraries: (1) Screenshots — paste UI screenshots and prompt AI to extract React + Tailwind components, use reflection technique to refine. (2) Chrome extensions — Magic Patterns extracts components directly from live web pages. (3) Code — use actual codebase components with mocked API responses for indistinguishable-from-production prototypes; Figma MCP server enables extracting design tokens into code. Two team workflows: Baselines and forks (reproduce current product as baseline, fork to explore variants without rebuilding), and product development lifecycle integration (discovery → roadmap/alignment → PRD/mocks → user interviews → engineering scoping). Introduces 'medium fidelity' concept — better than napkin sketches but not final Figma mocks. Practical tips: use Brandfetch or inspect-element for real logos, Unsplash for realistic images."
domain: professional-development
project: ai-pm
# taxonomy_inference: product-lifecycle/shape (prototyping-risk-reduction); ai-adoption (team-adoption, scaling-workflows)
# provenance: bulk-added by Claude from podcast-episode-compilation.md (2026-02-15)
# rescrape_needed: false — re-scraped from Lenny's Newsletter 2026-02-15
---

# How to Get Your Entire Team Prototyping with AI

**By**: Colin Matthews (guest post)
**Host**: Lenny Rachitsky
**Source**: [Lenny's Newsletter](https://www.lennysnewsletter.com/p/how-to-get-your-entire-team-prototyping)
**Type**: newsletter

## Summary

Comprehensive guide to scaling AI prototyping from individual exploration to team-wide adoption, by Colin Matthews (who has taught 500+ PMs and 10,000+ in online sessions). Addresses two key gaps: making prototypes look good enough for customers/stakeholders, and adopting tools as a team rather than individuals in silos. **Component libraries** (three methods): Screenshots — paste UI screenshots into AI tools to extract React + Tailwind components, use "reflection" technique to identify and fix differences. Chrome extensions — Magic Patterns extracts components directly from live web pages. Code — run front-end locally with mocked APIs for indistinguishable-from-production prototypes; new Figma MCP server enables extracting design tokens, CSS, and screenshots directly into Cursor. **Team workflows**: Baselines and forks — reproduce current product state as a baseline, then fork (free, no tokens) to explore variants without rebuilding. Product development lifecycle — prototypes at each stage with appropriate fidelity: mid-fi for discovery/internal communication, high-fi for stakeholder pitches and user interviews. **Key distinction**: code from AI prototyping tools is mostly useless to engineering teams (wrong patterns, libraries, sometimes wrong language) — prototypes serve as communication tools, not production code.

## Key Ideas Extracted

- **Component libraries as team infrastructure**: Up-front investment in shared components gives everyone building blocks for branded, consistent prototypes — screenshots, Chrome extensions, or real code depending on team capability
- **Reflection technique for UI refinement**: Ask AI to list differences between screenshot and implementation before asking it to fix — forces more accurate reproduction
- **Baselines and forks eliminate rebuild overhead**: Reproduce current product once as baseline, then fork freely to explore variants — each exploration costs zero tokens to start
- **Medium fidelity as new prototyping category**: AI tools create a middle tier between napkin sketches and polished Figma mocks — choosing appropriate fidelity for context prevents wasted effort
- **Prototype code is NOT production code**: AI-generated prototype code uses wrong patterns, libraries, and sometimes wrong languages — value is in communication, not code handoff; teams must set this expectation
- **Figma MCP server bridges design-to-code**: Cursor can autonomously take screenshots, extract design tokens, and get CSS from Figma's Dev Mode — very new but exciting for design teams
- **Fidelity should match audience**: Mid-fi for engineer handoff discussions, high-fi for CEO investment pitches and customer interviews — over-polishing wastes time, under-polishing undermines credibility
- **Prototypes drive better conversations than PRDs alone**: Showing a working prototype surfaces questions and edge cases faster than hoping engineers read the whole document

## Notes

- Published Jun 10, 2025 on Lenny's Newsletter. Guest post by Colin Matthews.
- Colin Matthews: PM at Datavant, has taught 5,000+ students, course "AI Prototyping for Product Managers"
- Tools covered: v0, Bolt, Cursor, Magic Patterns, Replit, Lovable, Windsurf, Figma MCP
- This is the sequel to his Jan 2025 guide "A guide to AI prototyping for product managers" (also in our sources)
- Includes detailed Reddit Answers example walking through full product development lifecycle
- Practical tips: Brandfetch for logos, SVG inspection, Unsplash for realistic placeholder images

## Raw Content

*Re-scraped from Lenny's Newsletter 2026-02-15. Full article content captured in Summary and Key Ideas above.*
