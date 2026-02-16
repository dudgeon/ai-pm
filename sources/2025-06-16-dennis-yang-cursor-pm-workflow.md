---
title: "How Dennis Yang Automates Product Management and Prototypes AI with Cursor"
created: 2026-02-15
updated: 2026-02-15
template: templates/source.md
template_version: 3
tags: [source, ai-pm, claude-added]
status: unread
source_type: podcast
source_url: "https://www.chatprd.ai/how-i-ai/ai-product-management-and-prototypes-with-cursor"
archive_url: ""
author: "Dennis Yang"
host: "Claire Vo"
published: 2025-10-27
discovered: 2026-02-15
summary: "Dennis Yang (Principal PM for Generative AI, Chime) on How I AI. Two workflows using Cursor as a central PM hub: (1) End-to-end PM lifecycle — writes PRDs in Markdown with Git version control, publishes to Confluence/Notion via MCPs, uses AI to read and draft responses to colleague comments with human-in-the-loop review, auto-generates detailed Jira epic and story tickets (with Gherkin acceptance criteria) from PRD context, automates weekly status reports via JQL queries with saved Cursor Rules for formatting; (2) 'Super MVP' AI agent prototyping — builds a Morning Briefing agent using plain English instructions in a Markdown file that Cursor executes as the runtime, chains MCPs (News API) without writing code, easily swaps underlying models (Claude, GPT-4, Gemini) to compare performance. Core insight: Cursor + MCPs turns a code editor into a PM's central nervous system where documentation, project management, and prototyping converge."
domain: professional-development
project: ai-pm
# taxonomy_inference: product-lifecycle/build (feature-specification-writing); horizontal/agents (prototyping); software-methodology (vibe-coding)
# provenance: bulk-added by Claude from podcast-episode-compilation.md (2026-02-15)
# rescrape_needed: false — re-scraped from ChatPRD 2026-02-16
---

# How Dennis Yang Automates Product Management and Prototypes AI with Cursor

**By**: Dennis Yang
**Host**: Claire Vo
**Source**: [How I AI (ChatPRD)](https://www.chatprd.ai/how-i-ai/ai-product-management-and-prototypes-with-cursor)
**Type**: podcast

## Summary

How I AI episode with Dennis Yang, Principal Product Manager for Generative AI at Chime. Dennis has completely rewired his PM workflow around Cursor, using it not for writing code but as a central hub for all PM work. Two detailed workflows: (1) End-to-end PM lifecycle — writes PRDs in Markdown with Git version control and Markdown Preview Enhanced extension, publishes to Confluence/Notion via MCPs with simple prompts, uses AI to read Confluence comments and draft categorized responses (High/Medium/Clarification priority) with human-in-the-loop approval, auto-generates Jira epic and story tickets with detailed Gherkin acceptance criteria from PRD context, automates weekly status reports via JQL queries with saved Cursor Rules for consistent formatting; (2) "Super MVP" AI agent prototyping — started with daily ChatGPT morning briefing prompt to build intuition, then built a customized Morning Briefing agent in Cursor using plain English instructions in a Markdown file that Cursor itself executes as the runtime, chains MCPs (News API search) without writing code, easily swaps underlying models (Claude, GPT-4, Gemini) to compare performance. Core insight: Cursor + MCPs turns a code editor into a PM's central nervous system where documentation, project management, and prototyping converge — the future is interoperability.

## Key Ideas Extracted

- **Cursor as PM central nervous system**: Use an AI IDE not for writing code but as a hub for writing PRDs, managing documentation, interacting with Jira/Confluence, and prototyping AI products
- **Markdown PRDs with Git version control**: Treat product documentation like source code — version control, change tracking, commit history, and the possibility of PRDs living adjacent to the code they describe
- **MCPs bridge Cursor to enterprise tools**: Connect to Confluence, Notion, Jira via Model Context Protocols — publish PRDs, read comments, create tickets, all from natural language prompts in Cursor
- **AI-assisted comment response with human review**: AI reads Confluence comments, categorizes by priority, drafts responses — PM reviews and approves, maintaining voice and accuracy while saving time
- **Automated Jira tickets from PRD context**: AI creates detailed epic and story tickets with Gherkin user stories and acceptance criteria because it has full PRD context — much richer than manual ticket creation
- **"Super MVP" agent prototyping**: Write plain English step-by-step instructions in a Markdown file, reference it in Cursor chat, and Cursor executes the instructions as an agent — the instructions ARE the application
- **Model comparison without code changes**: Swap Claude, GPT-4, Gemini as the underlying model in Cursor to compare agent performance — rapid experimentation for non-technical PMs
- **Cursor Rules for consistent formatting**: Save preferred report formats and styles as Cursor Rules for consistent, high-quality outputs from a single prompt

## Notes

- Published Oct 27, 2025 on How I AI (ChatPRD). ~9 min read. (Note: filename says 2025-06-16 but actual publication date is Oct 27, 2025)
- Sponsors: Zapier, Brex
- Dennis Yang background: Principal PM for Generative AI at Chime
- Tools: Cursor, MCPs (Confluence, Notion, Jira, News API), Git, Markdown Preview Enhanced extension, ChatGPT
- Key concept: "Super MVP" — super minimal viable product where instructions are the application
- Two companion workflow guides published Jan 8, 2026
- Cross-references: MCP architecture, PRD-adjacent-to-code concept, Cursor Rules

## Raw Content

*Re-scraped from ChatPRD 2026-02-16. Full article content captured in Summary and Key Ideas above.*
