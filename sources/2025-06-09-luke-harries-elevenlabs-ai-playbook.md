---
title: "3 AI Workflows to Save $140K & Automate Marketing with ElevenLabs' Luke Harries"
created: 2026-02-15
updated: 2026-02-15
template: templates/source.md
template_version: 3
tags: [source, ai-pm, claude-added]
status: unread
source_type: podcast
source_url: "https://www.chatprd.ai/how-i-ai/ai-workflows-to-automate-marketing-with-elevenlabs-luke-harries"
archive_url: ""
author: "Luke Harries"
host: "Claire Vo"
published: 2025-06-02
discovered: 2026-02-15
summary: "Luke Harries (Head of Growth, ElevenLabs) on How I AI. Three workflows for AI-native marketing: (1) Instant case studies — Granola AI transcription during customer interviews feeds a custom GPT copy editor with detailed brand voice instructions, producing polished case studies and tweet threads in under 15 minutes, connected to Salesforce via Zapier for pipeline automation; (2) Custom AI translation engine — built in Cursor over a weekend to replace $140K/year in localization SaaS and agencies, uses GitHub Actions to trigger LLM translation with language-specific prompt files containing brand guidelines and glossaries, zero maintenance cost; (3) WhatsApp MCP — open-source Model Context Protocol connecting WhatsApp messages to Claude via local SQLite database, enabling natural language queries over message history, summarization, and chained multi-tool agent workflows. Core philosophy: 'everything is a launch' — systematize and automate every part of marketing."
domain: professional-development
project: ai-pm
# taxonomy_inference: horizontal/agents (MCP-workflows); horizontal/runtimes (custom-GPTs); ai-adoption (tool-stack)
# provenance: bulk-added by Claude from podcast-episode-compilation.md (2026-02-15)
# rescrape_needed: false — re-scraped from ChatPRD 2026-02-16
---

# 3 AI Workflows to Save $140K & Automate Marketing with ElevenLabs' Luke Harries

**By**: Luke Harries
**Host**: Claire Vo
**Source**: [How I AI (ChatPRD)](https://www.chatprd.ai/how-i-ai/ai-workflows-to-automate-marketing-with-elevenlabs-luke-harries)
**Type**: podcast

## Summary

How I AI episode with Luke Harries, Head of Growth at ElevenLabs. Luke practices "vibe marketing" — AI as the engine for growth, automation, and efficiency, with a philosophy that "everything is a launch." Three workflows demonstrated: (1) Instant case studies with Granola and custom GPT — run Granola AI transcription during customer interviews, feed structured summary + raw transcript into a custom GPT copy editor loaded with detailed brand voice instructions (tone, formatting rules, positive examples), produces polished case study and tweet thread in under 15 minutes, connected to Salesforce via Zapier for automated outreach pipeline; (2) Custom AI translation engine replacing $140K/year — built in Cursor over a weekend by a non-engineer, uses GitHub Actions triggered by code changes to send strings to an LLM with language-specific prompt files containing brand guidelines, glossaries, and stylistic nuances, replaces $40K localization SaaS + $100K translation agencies with zero maintenance cost; (3) WhatsApp MCP — open-source Model Context Protocol connecting WhatsApp messages to Claude via local SQLite database using What's Meow library, enables natural language queries over message history, summarization of group chats, and chained multi-tool agent workflows (WhatsApp → Claude → ElevenLabs → WhatsApp voice note). Core insight: non-engineers can now build custom solutions that outperform expensive SaaS tools.

## Key Ideas Extracted

- **"Everything is a launch" philosophy**: Systematize and automate every part of marketing so high-quality work ships continuously — treat case studies, translations, and internal tools with the same rigor as product launches
- **Custom GPT as brand copy editor**: Don't use simple prompts — build detailed custom GPT instructions capturing entire tone of voice, formatting rules, and positive examples; edit the underlying prompt rather than correcting individual outputs
- **Granola for structured interview capture**: AI note-taker does more than transcribe — creates structured summaries, pulls key facts, enriches with context like job titles from email signatures
- **Non-engineer building production tools**: Marketer built a custom translation service in Cursor over a weekend — AI-assisted coding lets non-engineers build the first 90%, then work with engineering to polish and deploy
- **$140K SaaS replacement**: Custom AI translation engine replaced $40K/year localization software + $100K/year translation agencies with a GitHub Actions workflow and language-specific LLM prompts at near-zero cost
- **WhatsApp MCP for personal AI assistant**: Open-source MCP connecting WhatsApp to Claude — local SQLite database syncs messages, exposes functions like getRecentMessages and sendMessage to the AI
- **Chaining MCPs for autonomous agents**: WhatsApp MCP → Claude summarizes → ElevenLabs MCP generates voice note → WhatsApp MCP sends it back — demonstrates how connecting tools creates emergent agent capabilities
- **Pro tip: edit the prompt, not the output**: When AI makes recurring mistakes, fix the instructions in the custom GPT rather than correcting each output — compounds quality improvements over time

## Notes

- Published Jun 2, 2025 on How I AI (ChatPRD). ~9 min read. (Note: filename says 2025-06-09 but actual publication date is Jun 2, 2025)
- Sponsors: Orkes, Retool
- Luke Harries background: Head of Growth at ElevenLabs
- Tools: Granola (AI transcription), ChatGPT custom GPTs, Cursor, GitHub Actions, Zapier, Salesforce, WhatsApp MCP (What's Meow library), Claude, SQLite
- ElevenLabs plans to open-source their translation solution
- WhatsApp MCP is open-sourced on Luke's GitHub
- Three companion workflow guides published Jan 8, 2026
- Cross-references: MCP architecture, vibe coding for non-engineers, SaaS replacement thesis

## Raw Content

*Re-scraped from ChatPRD 2026-02-16. Full article content captured in Summary and Key Ideas above.*
