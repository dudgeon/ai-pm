---
title: "How I AI: Teresa Torres's Claude Code System for Task Management, Automated Research, and 'Lazy' Prompting"
created: 2026-02-05
updated: 2026-02-05
template: templates/source.md
template_version: 3
tags: [source, ai-pm]
status: unread
source_type: article
source_url: "https://www.chatprd.ai/how-i-ai/teresa-torres-claude-code-obsdian-task-management"
archive_url: "domains/professional-development/ai-pm/sources/2026-02-05-teresa-torres-claude-code-task-management.md"
author: "Teresa Torres"
host: "Claire Vo"
published: 2026-01-19
discovered: 2026-02-05
summary: "Teresa Torres (author, Continuous Discovery Habits) presents three deeply integrated Claude Code + Obsidian workflows: (1) Personalized task manager — custom /today slash command triggers Python script scanning task markdown files with YAML frontmatter, assembling daily to-do list with due/overdue/in-progress items and research digest. Tasks created via natural language, auto-tagged using taxonomy in claude.md. (2) Automated research digest — two Python cron jobs: morning script queries arXiv and Google Scholar with configured keywords, nightly script triggers Claude Code agents to summarize newly downloaded PDFs with focus on methodology and effect size. Summaries appear in next day's /today output. (3) 'Lazy prompting' via granular context library — broke single massive claude.md into dozens of tiny focused markdown files in an 'LLM Context' Obsidian vault with index files as maps; global claude.md routes business vs. personal queries to appropriate profiles. Built iteratively by asking Claude 'what'd you learn today that we should document?' at session end. Core thesis: pair programming for everything — most powerful AI apps are the ones you build for yourself."
domain: professional-development
project: ai-pm
# rescrape_needed: false — re-scraped from ChatPRD 2026-02-15
---

# How I AI: Teresa Torres's Claude Code System for Task Management, Automated Research, and 'Lazy' Prompting

**By**: Teresa Torres
**Host**: Claire Vo (ChatPRD)
**Source**: [ChatPRD - How I AI](https://www.chatprd.ai/how-i-ai/teresa-torres-claude-code-obsdian-task-management)
**Type**: article

## Summary

Three deeply integrated Claude Code + Obsidian workflows from Teresa Torres, who lives entirely in the terminal and describes her approach as "pair programming for everything." **Workflow 1 (Task Manager)**: Custom `/today` slash command triggers a Python script scanning all task markdown files (each with YAML frontmatter: type, due_date, tags) and assembles a daily to-do list with due/overdue/in-progress items plus research digest link. Tasks created via natural language in Claude Code terminal — Claude auto-tags using a taxonomy defined in claude.md. **Workflow 2 (Research Digest)**: Two Python cron jobs — morning script queries arXiv (daily) and Google Scholar (Sundays) with configured keywords; nightly script triggers Claude Code agents to summarize any newly downloaded PDFs, focusing on methodology and effect size. Summaries appear in next day's /today output. Led to a critical methodology review on LinkedIn that became one of her best-performing posts. **Workflow 3 (Lazy Prompting)**: Broke a single massive claude.md into dozens of tiny focused markdown files in an "LLM Context" Obsidian vault — separate folders for business and personal, with index files as maps (e.g., business_profile.md tells Claude where to find company overview, courses, partnerships). Global claude.md routes queries to appropriate profiles. Built iteratively by asking Claude "what'd you learn today that we should document?" at session end. Result: simple prompts like "Claude blog post review, gimme feedback" produce high-quality output because context is pre-loaded and well-organized.

## Key Ideas Extracted

- **Pair programming for everything**: Claude Code as true partner across all workflows (tasks, writing, research), not just a code tool — navigates her entire computer through the terminal
- **Custom slash commands as workflow entry points**: `/today` kicks off the entire daily system — one command, full context assembly, zero GUI friction
- **Tasks as individual markdown files**: Each task is its own file with YAML frontmatter, making data portable, searchable, and fully accessible to LLMs — superior to locked-in task management tools
- **Manual download as intentional filter**: In the research pipeline, human PDF download step prevents information overload — automation handles discovery and summarization, human handles curation
- **Granular context > monolithic context**: Breaking context into dozens of tiny focused files with index maps beats a single large claude.md — prevents irrelevant context loading and enables intelligent routing
- **Iterative context building**: "What'd you learn today that we should document?" at session end turns every interaction into a context-improvement opportunity — the system gets smarter over time
- **AI-powered thought leadership**: Automated research digest enabled rapid critical analysis of a new paper, producing a high-performing LinkedIn post — AI creates opportunities, not just efficiencies
- **Build your own tools thesis**: The most powerful AI applications may be the ones built for individual workflows — friction of generic tools is the opportunity cost

## Notes

- Published Jan 19, 2026 on ChatPRD blog. 9-min read.
- Tools: Claude Code, Obsidian, VS Code, Descript, ChatGPT, Trello (replaced)
- Teresa Torres is author of Continuous Discovery Habits — internationally recognized product coach
- Links: producttalk.org (blog), justnowpossible.com (podcast)
- Her system is highly relevant to our home-brain architecture — similar philosophy of markdown-first, context libraries, and CLI-driven workflows
- Sponsors: Brex, Graphite (AI code review platform)
- Cross-reference: The granular context library approach parallels our own .claude/ philosophy.md + communication.md + context-management.md structure

## Raw Content

*Re-scraped from ChatPRD 2026-02-15. Full article content captured in Summary and Key Ideas above.*
