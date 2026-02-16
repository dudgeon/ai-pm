---
title: "Zach Davis's 3 Workflows for Enterprise Engineering with AI"
created: 2026-02-15
updated: 2026-02-16
template: templates/source.md
template_version: 3
tags: [source, ai-pm, claude-added]
status: unread
source_type: podcast
source_url: "https://www.chatprd.ai/how-i-ai/enterprise-engineering-with-ai"
archive_url: ""
author: "Zach Davis"
host: "Claire Vo"
published: 2025-07-21
discovered: 2026-02-15
summary: "Zach Davis (Director of Engineering, LaunchDarkly) on How I AI. Three workflows for weaving AI into enterprise engineering processes: (1) Centralizing documentation for humans and AI agents — created a docs directory in monorepo organized by category, consolidated from Confluence/Google Docs, created unified do_agents_rules directory with universal rules that tool-specific files (.cursor, .devon) reference, used Augment to generate rule files, iteratively improved by identifying where agents were struggling; (2) AI-powered tech debt reduction — ran yarn test piped to log file, used Claude to analyze logs and categorize issues by type/severity, generated prioritized markdown checklist in agents/migrations directory, assigned tasks to Cursor/Devin/other agents one at a time, review and merge cycle; (3) AI-powered hiring process improvement — created detailed interview rubric, built custom GPT with rubric + examples of excellent/poor scorecards, evaluates interviewer submissions and generates feedback with strengths/areas for improvement plus Slack-ready summary. Core insight: building solid, scalable AI processes for engineering teams — not just shortcuts, but workflows that help both human engineers and AI agents."
domain: professional-development
project: ai-pm
# taxonomy_inference: ai-adoption (enterprise-adoption); horizontal/context (documentation-for-agents); software-methodology (compound-engineering)
# provenance: bulk-added by Claude from podcast-episode-compilation.md (2026-02-15)
# rescrape_needed: false — re-scraped from ChatPRD 2026-02-16
---

# Zach Davis's 3 Workflows for Enterprise Engineering with AI

**By**: Zach Davis
**Host**: Claire Vo
**Source**: [How I AI (ChatPRD)](https://www.chatprd.ai/how-i-ai/enterprise-engineering-with-ai)
**Type**: podcast

## Summary

How I AI episode with Zach Davis, Director of Engineering at LaunchDarkly. Three workflows showing how to weave AI into day-to-day engineering processes in a large org with a massive codebase — beyond "vibe coding" into solid, scalable workflows: (1) Centralizing documentation for humans and AI agents — created a docs directory within the monorepo organized by category (frontend, backend, accessibility), consolidated from scattered Confluence/Google Docs sources, built a unified do_agents_rules directory with universal rules that tool-specific files (.cursor rules, .devon files) simply reference, used Augment to generate the centralized rule files, iteratively improved rules by identifying where AI agents were previously struggling; (2) AI-powered tech debt reduction — ran `yarn test` piped to a log file to identify noisy console logs, used Claude to analyze the log and categorize issues by type and severity, generated a prioritized markdown checklist in agents/migrations directory, assigned individual tasks to Cursor, Devin, and other agents one at a time, review-and-merge cycle with task completion tracking; (3) AI-powered hiring process improvement — created a detailed interview evaluation rubric, built a custom GPT with the rubric plus examples of excellent and poor scorecards, evaluates interviewer submissions and rates them (Excellent/Good/Fair/Poor) with specific feedback on strengths and areas for improvement, generates concise Slack messages for delivering feedback efficiently.

## Key Ideas Extracted

- **Centralized docs directory as single source of truth**: Put all documentation in one monorepo directory organized by category — both engineers and AI agents reference the same up-to-date information instead of scattered Confluence/Google Docs
- **Unified agent rules with tool-specific references**: Create universal rules in a central do_agents_rules directory, then have tool-specific files (.cursor, .devon) reference the relevant central files — avoids maintaining duplicate rule sets
- **AI-generated rule files with iterative improvement**: Use Augment to generate initial rule files, then improve by identifying specific areas where agents were struggling — makes agents more efficient out of the gate
- **Test log analysis for systematic tech debt reduction**: Pipe `yarn test` output to a log file, use Claude to categorize issues by type/severity, generate a prioritized markdown checklist that agents can work through one task at a time
- **Agents/migrations directory pattern**: Store AI-generated task lists in a dedicated agents/migrations directory within the codebase — gives the tech debt reduction process a clear, trackable home
- **Custom GPT for interview feedback consistency**: Provide a rubric + examples of excellent and poor scorecards in a custom GPT prompt — standardizes evaluation quality and produces Slack-ready feedback summaries
- **Workflows for both humans and agents**: Design processes that help both human engineers and AI agents — centralized docs serve double duty, improving human discoverability while giving agents accurate context
- **Scalable AI processes over shortcuts**: Focus on repeatable, team-wide workflows (documentation, tech debt, hiring) rather than individual productivity hacks — the real value is in building institutional capability

## Notes

- Published Jul 21, 2025 on How I AI (ChatPRD). ~5 min read. (Note: filename says 2025-09-15 but actual publication date is Jul 21, 2025)
- Sponsors: WorkOS, Lenny's List
- Zach Davis background: Director of Engineering at LaunchDarkly
- Tools: Augment (rule generation), Claude (log analysis), Cursor (agent tasks), Devin (agent tasks), custom GPT (hiring feedback)
- Key pattern: Monorepo docs directory with unified agent rules that tool-specific configs reference
- Three companion workflow guides published Jan 8, 2026
- Cross-references: Enterprise AI adoption, documentation-for-agents pattern, AI-assisted tech debt, AI in hiring

## Raw Content

*Re-scraped from ChatPRD 2026-02-16. Full article content captured in Summary and Key Ideas above.*
