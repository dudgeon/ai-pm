---
title: "Terry Lin's Vibe Coding Workflow for Building an Apple Watch Fitness App"
created: 2026-02-15
updated: 2026-02-15
template: templates/source.md
template_version: 3
tags: [source, ai-pm, claude-added]
status: unread
source_type: podcast
source_url: "https://www.chatprd.ai/how-i-ai/vibe-coding-apple-watch-fitness-app"
archive_url: ""
author: "Terry Lin"
host: "Claire Vo"
published: 2025-09-15
discovered: 2026-02-15
summary: "Terry Lin (PM, vibe coder) on How I AI. Two workflows for building Cooper's Corner, a voice-powered fitness app for iPhone/Apple Watch: (1) Structured vibe coding — 'dual-wielding' Cursor (AI coding) + Xcode (compiling/debugging); three-phase AI workflow with custom Cursor Rules: PRD Create (Linear ticket → full PRD with Gherkin user stories), PRD Review (second AI rates plan 9+/10 before execution), PRD Execute (break into phased checklist with git commits after each phase); 'vibe refactoring' to keep files under 400 lines for better AI collaboration; 'Rubber Duck' rule where AI explains and quizzes you on code it wrote; (2) Index card prototyping — sketch UI on index cards (phone aspect ratio), photograph and upload to GPT-4 Vision with 'help me upscale this', bring AI-generated mockup into UX Pilot → Figma with Apple UI Kit. V1 was just Apple Watch voice memos → Python script → GPT-4 → Excel to prove concept before building the real app."
domain: professional-development
project: ai-pm
# taxonomy_inference: software-methodology (vibe-coding); product-lifecycle/shape (prototyping-risk-reduction)
# provenance: bulk-added by Claude from podcast-episode-compilation.md (2026-02-15)
# rescrape_needed: false — re-scraped from ChatPRD 2026-02-16
---

# Terry Lin's Vibe Coding Workflow for Building an Apple Watch Fitness App

**By**: Terry Lin
**Host**: Claire Vo
**Source**: [How I AI (ChatPRD)](https://www.chatprd.ai/how-i-ai/vibe-coding-apple-watch-fitness-app)
**Type**: podcast

## Summary

How I AI episode with Terry Lin, product manager and vibe coder. Two workflows for building Cooper's Corner, a voice-powered fitness tracker for iPhone and Apple Watch: (1) Structured vibe coding process — "dual-wielding" Cursor (for AI-assisted coding) + Xcode (for compiling, simulator, debugging); strict three-phase AI cycle with custom Cursor Rules: PRD Create (takes Linear ticket → full PRD with goals, references, Gherkin user stories), PRD Review (second AI agent rates plan out of 10, keeps iterating until 9+), PRD Execute (breaks work into phased checklist, git commit after each phase for easy rollback); "vibe refactoring" rule to keep files under 400 lines by splitting "God mode" files so AI works more efficiently; "Rubber Duck" rule where AI explains new code and creates pop quizzes to ensure learning; (2) Index card prototyping — sketch mobile UI on physical index cards (approximates phone aspect ratio), photograph with phone camera, upload to GPT-4 Vision with "help me upscale this," bring AI-generated mockup into UX Pilot → Figma with Apple's official UI Kit. Started with a scrappy V1: Apple Watch voice memos → Python script → GPT-4 transcription → structured Excel data, proving the concept before building a real app.

## Key Ideas Extracted

- **Three-phase AI workflow: Create, Review, Execute**: Custom Cursor Rules for each phase — PRD Create builds full spec from ticket, PRD Review has AI score the plan 9+/10 before coding starts, PRD Execute breaks work into phased checklist with git commits
- **"Dual-wielding" Cursor + Xcode**: Cursor for AI-assisted code generation, Xcode for compiling, simulator testing, and catching build-specific errors — necessary for iOS development
- **Vibe refactoring for AI optimization**: Keep files under 400 lines by splitting large files — LLMs waste tokens reading oversized files, smaller files = more efficient AI collaboration
- **Rubber Duck rule for learning**: AI explains its own code and creates pop quizzes — ensures the builder understands what was generated, not just along for the ride
- **PRD Review as quality gate**: Second AI agent reviews the plan and rates it out of 10 — prevents garbage-in/garbage-out by ensuring instructions are clear before execution
- **Git commits as risk management**: AI pauses after each execution phase and commits — creates a trail of small changes for easy rollback, builds trust for more complex tasks
- **Index card → GPT-4 Vision → Figma pipeline**: Physical sketches on index cards → AI upscaling → UX Pilot → Figma with native UI Kit — go from subway idea to polished prototype in minutes
- **Start with the scrappiest V1 possible**: Voice memos → Python → Excel proved the concept before any app development — classic PM discipline applied to vibe coding

## Notes

- Published Sep 15, 2025 on How I AI (ChatPRD). ~9 min read. (Note: filename says 2025-07-28 but actual publication date is Sep 15, 2025)
- Sponsors: Paragon, Miro
- Terry Lin background: Product manager, vibe coder, self-described "AI-powered gym bro"
- Tools: Cursor, Xcode, Linear, GPT-4 Vision, Figma, UX Pilot, Apple UI Kit, Python, Apple Watch voice memos
- App: Cooper's Corner — voice-powered fitness tracker for iPhone + Apple Watch
- Key concept: "Vibe refactoring" — clean up code for AI, not just humans
- Two companion workflow guides published Jan 8, 2026
- Cross-references: Cursor Rules, structured vibe coding, mobile development with AI

## Raw Content

*Re-scraped from ChatPRD 2026-02-16. Full article content captured in Summary and Key Ideas above.*
