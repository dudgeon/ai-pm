---
created: 2026-02-17
updated: 2026-02-17
template: templates/source.md
template_version: 3
tags: [source, ai-pm]
status: unread
source_type: article
source_url: "https://every.to/source-code/i-stopped-reading-code-my-code-reviews-got-better"
archive_url: "domains/professional-development/ai-pm/sources/2026-01-23-i-stopped-reading-code-reviews-got-better.md"
author: "Kieran Klaassen"
published: 2026-01-23
discovered: 2026-02-17
summary: "Kieran Klaassen stops reading code line-by-line in reviews and gets better results: a 1,000-line, 27-file bug fix gets reviewed by having Claude Code summarize what changed and why, using the compound engineering plugin to extract 'findings' that become decisions for future sessions. The 50/50 rule: spend half review time on business logic (what it does), half on architectural decisions (why it's structured that way). The fix is never the last fix — the AI surfaces related issues automatically."
domain: professional-development
project: ai-pm
scraped_by: claude
---

# I Stopped Reading Code. My Code Reviews Got Better.

**By**: Kieran Klaassen
**Source**: [Original URL](https://every.to/source-code/i-stopped-reading-code-my-code-reviews-got-better)
**Type**: article

## Summary

*Fill after reading with your own take.*

## Key Ideas Extracted

*Fill during processing.*

## Notes

*Your annotations, reactions, questions, disagreements.*

## Raw Content

**I Stopped Reading Code. My Code Reviews Got Better.**

By Kieran Klaassen | January 23, 2026 | Source Code

A bug report: email signature formatting was off in Cora. Kieran asked Claude Code to investigate and fix it. By morning, the fix had touched 27 files, 1,000+ lines of code. Instead of reading it all, he had Claude summarize what changed and why.

Key sections:
- **The death of manual code review**: Claude Code does the reading; human reviews the summary and decisions
- **Using the compound engineering plugin**: Extracts "findings" from each review session
- **From findings to decisions**: Findings get encoded as rules for future sessions
- **The fix is never the last fix**: AI surfaces related issues automatically during review
- **The 50/50 rule**: Split review time 50% on business logic (what it does), 50% on architectural decisions (why it's structured that way)
- **Rethink reviews**: Code review becomes "architectural review" — you're reviewing decisions, not lines

Core insight: When AI writes all your code, your job in review is to evaluate decisions and encode lessons, not to verify syntax and logic line-by-line.
