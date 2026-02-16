---
title: "Automate Recruiting and Build Interactive Personas with Michal Peled of HoneyBook"
created: 2026-02-15
updated: 2026-02-16
template: templates/source.md
template_version: 3
tags: [source, ai-pm, claude-added]
status: unread
source_type: podcast
source_url: "https://www.chatprd.ai/how-i-ai/recruiting-and-ai-personas"
archive_url: ""
author: "Michal Peled"
host: "Claire Vo"
published: 2025-12-08
discovered: 2026-02-15
summary: "Michal Peled (Technical Operations Engineer, HoneyBook) on How I AI. Three 'little helper' workflows: (1) LinkedIn recruiting agent with ChatGPT agent mode — structured prompt gives AI a recruiter role with detailed constraints (location, activity recency, tenure requirements), agent opens browser to navigate LinkedIn, search, filter, and vet profiles; returns formatted table with 5 candidates and match scores in ~10 minutes; 4/5 were new high-quality prospects the team hadn't found manually, 1/5 was already in their pipeline (validating accuracy); includes collaborative handoff for login ('let me take control'); (2) Interactive AI personas from static customer research — uploaded hundreds of pages of buyer persona research into NotebookLM (chose for source-grounded answers and citations); prompted NotebookLM as 'expert prompt engineer' to generate custom GPT prompts for 5 distinct personas; refined with ChatGPT/Claude to fit 8,000-char limit and add guardrails (no off-topic, respectful, no political/religious content); each persona gives distinct, in-character responses to product/marketing questions; (3) Game-day parking calendar — single ChatGPT prompt generates ICS file of all weekday daytime Giants home games, imports to Google Calendar as all-day events with 'free' availability, shared with team to avoid $40+/hour surge parking near Oracle Park. Core insight: internal tools teams are innovation centers — identify recurring friction points and build 'little helpers' with the right-sized AI tool."
domain: professional-development
project: ai-pm
# taxonomy_inference: horizontal/agents (agent-building); horizontal/runtimes (NotebookLM); product-lifecycle/discover (problem-signal-detection)
# provenance: bulk-added by Claude from podcast-episode-compilation.md (2026-02-15)
# rescrape_needed: false — re-scraped from ChatPRD 2026-02-16
---

# Automate Recruiting and Build Interactive Personas with Michal Peled of HoneyBook

**By**: Michal Peled
**Host**: Claire Vo
**Source**: [How I AI (ChatPRD)](https://www.chatprd.ai/how-i-ai/recruiting-and-ai-personas)
**Type**: podcast

## Summary

How I AI episode with Michal Peled, Technical Operations Engineer at HoneyBook. Three "little helper" workflows demonstrating practical AI for internal tools: (1) LinkedIn recruiting agent with ChatGPT agent mode — crafted a structured prompt by interviewing recruiters about their step-by-step workflow, gives the AI a recruiter role with specific constraints (candidates from Israel or Israeli companies, active within 3 months, matching title and seniority, 1+ year tenure or recently unemployed); agent mode opens a "magic computer" browser window to navigate LinkedIn, search profiles, apply filters, and vet candidates; "thoughts" panel shows real-time reasoning; returns formatted table with 5 candidates, profile links, and match scores in ~10 minutes; validation showed 4/5 were new high-quality prospects never found manually, 1/5 was already in the interview pipeline (confirming accuracy); includes collaborative handoff for login; (2) Interactive AI personas from static customer research — uploaded hundreds of pages of buyer persona research documents into NotebookLM (chose for source-grounded answers with citations); prompted NotebookLM as "expert prompt engineer" to read all research and generate detailed custom GPT prompts for 5 distinct personas; included strict instruction not to add or modify information beyond the source; refined prompts with ChatGPT and Claude to fit 8,000-character limit and add guardrails (no off-topic, no slang, no political/religious content); created 5 custom GPTs that give distinct in-character responses to product and marketing questions; (3) Game-day parking calendar automation — single ChatGPT prompt finds all Oracle Park home games in next 6 months, filters to morning-2PM starts, generates downloadable ICS file as all-day events with "free" availability and game details in description; imported to Google Calendar and shared with team; solved recurring $40+/hour surge parking problem in 36 seconds.

## Key Ideas Extracted

- **Agent mode as collaborative co-pilot**: Instruct the agent what to do autonomously but include handoff points ("let me take control and log in") — agents don't have to be fire-and-forget
- **Interview the experts to write the prompt**: Map out the exact human workflow step-by-step by talking to the people who do the job, then translate directly into an AI prompt — produces much better results than generic instructions
- **"Thoughts" panel for agent transparency**: ChatGPT agent mode shows real-time reasoning ("Now I will go to the feed page," "I plan to click on...") — builds trust and helps debug agent behavior
- **NotebookLM for source-grounded prompt generation**: Use NotebookLM's citation-backed, source-only mode to generate custom GPT prompts from research docs — prevents the AI from inventing persona details not in the research
- **Meta-prompting: AI as prompt engineer**: Prompt one AI tool to generate prompts for another AI tool — NotebookLM reads research and creates the custom GPT system prompts, a more reliable pipeline than writing them manually
- **Guardrails for enterprise custom GPTs**: Add explicit constraints (no off-topic responses, respectful tone, no political/religious content) — should be a default for all enterprise-facing AI personas
- **Right-sized AI for right-sized problems**: Complex recruiting → agent mode; static research → NotebookLM + custom GPTs; parking schedule → single prompt with ICS file output — match the tool complexity to the problem complexity
- **Internal tools teams as AI innovation centers**: Technical ops/internal tools teams can often move faster than customer-facing product teams because they face less red tape and can directly solve their colleagues' daily friction

## Notes

- Published Dec 8, 2025 on How I AI (ChatPRD). ~9 min read. (Note: filename says 2025-10-20 but actual publication date is Dec 8, 2025)
- Sponsors: Brex, Google Gemini
- Michal Peled background: Technical Operations Engineer at HoneyBook; builds internal tools and automations
- Tools: ChatGPT (agent mode for recruiting, ICS generation), NotebookLM (source-grounded persona generation), Claude (prompt refinement), Custom GPTs (5 interactive personas), Google Calendar
- Key stats: 5 candidates found in ~10 minutes; 4/5 new high-quality; ICS file generated in 36 seconds
- HoneyBook office: near Oracle Park (SF Giants), hence the parking problem
- Three companion workflow guides published Jan 8, 2026
- Cross-references: Agent mode workflows, interactive personas, NotebookLM, internal tools innovation, recruiting automation

## Raw Content

*Re-scraped from ChatPRD 2026-02-16. Full article content captured in Summary and Key Ideas above.*
