---
title: "Tim McAleer's AI Workflows for Documentary Filmmaking at Florentine Films"
created: 2026-02-15
updated: 2026-02-16
template: templates/source.md
template_version: 3
tags: [source, ai-pm, claude-added]
status: unread
source_type: podcast
source_url: "https://www.chatprd.ai/how-i-ai/ai-workflows-for-documentary-filmmaking"
archive_url: ""
author: "Tim McAleer"
host: "Claire Vo"
published: 2025-11-17
discovered: 2026-02-15
summary: "Tim McAleer (producer, Ken Burns' Florentine Films) on How I AI. Three custom AI tools for documentary post-production: (1) AI-powered media database — built Python script in Cursor (dictated via Super Whisper) using OpenAI Vision API to auto-describe archival images; enhanced accuracy by scraping EXIF metadata as factual guardrails; expanded to video (frame sampling every 5 sec → cheap model captions + Whisper audio transcription → advanced model summary) and audio; implemented semantic search via vector embeddings (CLIP for images + OpenAI text embeddings, fused into multi-modal vectors) enabling reverse image search across 20,000+ assets; (2) 'Flip Flop' iOS app for field research — vibe-coded with ChatGPT (PRD) → Claude (Swift UI code); captures front/back of archival documents, sends to OpenAI API for description and handwriting transcription, embeds all generated data into EXIF metadata making each photo self-contained; fixes the chaos of 1,400 unorganized research photos; (3) 'OCR Party' Mac menu bar app — precision OCR tool that lets users crop specific regions of complex documents (old newspapers, damaged letters, faded cursive) and submit just that portion for AI analysis; handles creases, ink blots, faded text. Core insight: AI automates the tedious parts of documentary research (data entry, cataloging, transcription) to amplify creativity, not replace it."
domain: professional-development
project: ai-pm
# taxonomy_inference: horizontal/agents (domain-specific-agents, custom-tool-building); software-methodology (vibe-coding)
# provenance: bulk-added by Claude from podcast-episode-compilation.md (2026-02-15)
# rescrape_needed: false — re-scraped from ChatPRD 2026-02-16
---

# Tim McAleer's AI Workflows for Documentary Filmmaking at Florentine Films

**By**: Tim McAleer
**Host**: Claire Vo
**Source**: [How I AI (ChatPRD)](https://www.chatprd.ai/how-i-ai/ai-workflows-for-documentary-filmmaking)
**Type**: podcast

## Summary

How I AI episode with Tim McAleer, producer at Ken Burns' Florentine Films. Three custom AI tools solving documentary post-production bottlenecks: (1) AI-powered media database with REST API — started with simple Python script in Cursor (dictated via Super Whisper voice-to-text) using OpenAI Vision API to describe archival images; enhanced accuracy by scraping EXIF metadata from files (photographer, date, location from Library of Congress sources) and passing it as factual guardrails alongside the image; expanded to video processing (frame sampling every 5 seconds for cost efficiency → cheap model like GPT-4-nano for frame captions + Whisper for audio transcription in 5-second chunks → advanced model weaves all together into complete summary); implemented semantic search via fused vector embeddings (CLIP for image thumbnails + OpenAI text model for descriptions, combined into multi-modal vectors) enabling reverse image search ("Find Similar" button) across 20,000+ assets to discover thematic connections; (2) "Flip Flop" custom iOS app for field research in physical archives — vibe-coded with ChatGPT generating PRD from screen/flow description, Claude writing Swift UI code in single shot; captures front of document then immediately flips to capture back; sends both to OpenAI API (front gets visual description, back gets handwriting transcription); embeds all generated data directly into image EXIF metadata making each photo self-contained and database-ready; solves the chaos of returning from archives with 1,400 unorganized front/back photos; (3) "OCR Party" Mac menu bar utility — precision OCR tool for complex/damaged historical documents; user opens document image, draws cropping box around specific region (single article in dense newspaper, paragraph, handwritten name), submits just that crop to AI; handles creases, ink blots, faded text, partially obscured words, and difficult cursive; returns clean text with crop coordinates for source reference.

## Key Ideas Extracted

- **EXIF metadata as AI factual guardrails**: Scrape embedded metadata (photographer, date, location) from archival photos and pass alongside the image to the vision model — transforms generic descriptions into factually grounded, documentary-quality captions
- **Cost-optimized video analysis pipeline**: Sample frames every 5 seconds (not every frame), use cheap model for frame captions, Whisper for audio in 5-second chunks, then bundle everything for one advanced model pass — balances quality with cost at scale
- **Fused multi-modal vector embeddings**: Combine CLIP image embeddings with OpenAI text embeddings into a single vector per asset — enables reverse image search ("Find Similar") that finds assets by visual style, subject, or thematic connection
- **Self-contained image files via EXIF embedding**: Write AI-generated descriptions, transcriptions, and collection context directly into image EXIF metadata — each photo becomes a data-rich asset that carries its own context regardless of where it's stored
- **Vibe-coded iOS app with ChatGPT + Claude pipeline**: Describe screens and user flow → ChatGPT generates PRD → Claude writes Swift UI code in single shot — non-engineer built a functional field research app
- **Region-specific OCR for complex documents**: Crop just the relevant section instead of processing the whole page — dramatically improves accuracy for dense newspapers, multi-column layouts, and damaged historical materials
- **Voice-to-text for initial coding prompts**: Super Whisper dictation into Cursor lets you describe what you want built conversationally — lower barrier than typing formal specifications
- **AI automates toil to amplify creativity**: Documentary teams go from copying and pasting text to discovering thematic connections across tens of thousands of data points — the tedious work disappears so storytelling improves

## Notes

- Published Nov 17, 2025 on How I AI (ChatPRD). ~10 min read. (Note: filename says 2025-10-13 but actual publication date is Nov 17, 2025)
- No sponsors listed in article
- Tim McAleer background: Producer at Ken Burns' Florentine Films; in charge of tech and processes for documentary production
- Tools: Cursor (coding), Super Whisper (voice-to-text), OpenAI Vision API, Whisper (audio transcription), CLIP (image embeddings), OpenAI text embeddings, ChatGPT (PRD generation), Claude (Swift code), Python, Airtable
- Scale context: Muhammad Ali series = 20,000+ still images, hundreds of hours of footage
- Custom apps: "Flip Flop" (iOS field research), "OCR Party" (Mac menu bar OCR)
- Three companion workflow guides published Jan 8, 2026
- Cross-references: Vibe coding custom tools, vector embeddings for search, documentary/media workflows, physical archive digitization

## Raw Content

*Re-scraped from ChatPRD 2026-02-16. Full article content captured in Summary and Key Ideas above.*
