---
title: "Vibe Coding a 3D Multiplayer Game in 15 Minutes—With No Game Dev Experience"
created: 2026-02-15
updated: 2026-02-15
template: templates/source.md
template_version: 3
tags: [source, ai-pm, claude-added]
status: unread
source_type: podcast
source_url: "https://www.chatprd.ai/how-i-ai/vibe-code-3d-multiplayer-game-in-15-minutes"
archive_url: ""
author: "Cody De Arkland"
host: "Claire Vo"
published: 2025-05-05
discovered: 2026-02-15
summary: "Cody De Arkland (Sr. Dir DevEx, Sentry) on How I AI. Two workflows demonstrated: (1) Deconstructing his 'Spaceflight' multiplayer space game — built iteratively with zero game dev experience using Cursor and Claude as junior developer partners, learning 3D concepts (Three.js, GLTF models, WebSockets) from the AI as he went; (2) Live speedrun building a brand new 3D multiplayer flight simulator from blank folder to playable prototype in ~15 minutes using Claude Code CLI with --yolo flag, parallel front-end/back-end development in separate terminal sessions. Key insight: vibe coding is about being a creative director for a fast, sometimes chaotic junior developer — give broad creative prompts, iterate conversationally on what AI produces, guide toward your goal. Same principles apply to enterprise software at Sentry."
domain: professional-development
project: ai-pm
# taxonomy_inference: software-methodology (vibe-coding)
# provenance: bulk-added by Claude from podcast-episode-compilation.md (2026-02-15)
# rescrape_needed: false — re-scraped from ChatPRD 2026-02-16
---

# Vibe Coding a 3D Multiplayer Game in 15 Minutes—With No Game Dev Experience

**By**: Cody De Arkland
**Host**: Claire Vo
**Source**: [How I AI (ChatPRD)](https://www.chatprd.ai/how-i-ai/vibe-code-3d-multiplayer-game-in-15-minutes)
**Type**: podcast

## Summary

How I AI episode with Cody De Arkland, Senior Director of Developer Experience at Sentry. Two demonstrations: (1) Deconstructing "Spaceflight" — a fully functional multiplayer 3D space game built iteratively with zero game dev experience, treating AI (Cursor + Claude) as a junior developer partner; learned 3D concepts like Three.js, GLTF/GLB models, and WebSockets from the AI as he went; overcame challenges like model orientation (AI needed very precise spatial instructions) and multiplayer race conditions (AI caught them during code review); (2) Live speedrun — builds a brand new 3D multiplayer flight simulator from blank folder to playable prototype in ~15 minutes; uses Claude Code CLI with --yolo flag for autonomous execution, runs parallel sessions (front-end fixes in one terminal, back-end multiplayer in another), starts with broad creative prompts and iterates conversationally on output. Key takeaway: vibe coding is less about writing perfect code and more about being a creative director for a fast, sometimes chaotic junior developer — give broad creative prompts, iterate on what AI produces, guide toward your goal. Same principles apply to enterprise software at Sentry.

## Key Ideas Extracted

- **Treat AI as a junior developer partner**: Don't write detailed specs — describe the vibe, iterate conversationally, guide toward your goal; the AI is a fast but imperfect collaborator
- **Zero-to-complex is now accessible**: Built a multiplayer 3D space game with zero game dev experience — the barrier to creating complex, ambitious software has never been lower
- **15-minute speedrun from blank folder**: Live demo building a 3D multiplayer flight simulator from scratch using Claude Code CLI — proves the speed isn't exaggerated
- **Parallel development sessions**: Run separate Claude Code instances for front-end and back-end simultaneously — multiplayer backend being built while front-end bugs are being fixed
- **Claude Code --yolo flag for autonomous execution**: Gives AI permission to make any changes without confirmation — enables rapid iteration but requires trust
- **AI as learning tool, not just coding tool**: Used AI to explain 3D concepts (Three.js, GLTF models, WebSockets) while building — learned by building rather than studying first
- **Precision matters for spatial/visual tasks**: Model orientation required very specific prompts ("the front of the ship is a 90-degree turn to the left horizontally") — abstract descriptions fail for visual work
- **AI catches bugs during code review**: During multiplayer implementation, AI identified potential race conditions and optimization issues — acting as both builder and reviewer
- **Vibe coding applies to enterprise software too**: Same iterative, conversational approach works for Sentry day job, not just personal projects

## Notes

- Published May 5, 2025 on How I AI (ChatPRD). ~8 min read.
- Sponsors: Enterpret, WorkOS
- Cody De Arkland background: Sr. Director Developer Experience at Sentry; prolific vibe coder building personal productivity apps and complex workflows
- Tools: Cursor, Claude Code CLI (--yolo flag), Three.js, SketchFab (3D models), WebSockets/Socket.io, React (Vite template)
- Game "Spaceflight" — multiplayer space flight simulator inspired by X-Wing and No Man's Sky
- Live demo game "boop-flight" — low-poly flight simulator with multiplayer and chat
- Two companion workflow guides published Jan 8, 2026
- Cross-references: Vibe coding (Andrej Karpathy coined term), Claude Code techniques (John Lindquist episode)

## Raw Content

*Re-scraped from ChatPRD 2026-02-16. Full article content captured in Summary and Key Ideas above.*
