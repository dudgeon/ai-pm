---
title: "3 Advanced Codex Workflows: Git Worktrees, Plans.md, and Automated Code Reviews"
created: 2026-02-15
updated: 2026-02-15
template: templates/source.md
template_version: 3
tags: [source, ai-pm, claude-added]
status: unread
source_type: podcast
source_url: "https://www.chatprd.ai/how-i-ai/advanced-codex-workflows-with-openai-alex-embiricos"
archive_url: ""
author: "Alexander Embiricos"
host: "Claire Vo"
published: 2026-01-12
discovered: 2026-02-15
summary: "Alexander Embiricos (Product Lead, Codex, OpenAI) presents four workflows progressing from beginner to advanced: (1) Zero-to-one — use Codex to understand unfamiliar codebases and make natural-language changes. (2) Git worktrees for parallel development — Codex creates worktrees via terminal commands, enabling isolated parallel tasks without merge conflicts. (3) Plans.md technique — create a meta-plan template that instructs the model how to generate implementation plans with self-contained milestones; used to ship Sora Android app in 28 days. (4) Automated GitHub code review — Codex scans PRs, only flags high-confidence issues, engineers reply to fix in-thread. Used on almost every OpenAI repo."
domain: professional-development
project: ai-pm
# taxonomy_inference: horizontal/agents (Codex, agent-workflows); horizontal/context (Plans.md-as-context); software-methodology (compound-engineering)
# provenance: bulk-added by Claude from podcast-episode-compilation.md (2026-02-15)
# rescrape_needed: false — re-scraped from ChatPRD 2026-02-15
---

# 3 Advanced Codex Workflows: Git Worktrees, Plans.md, and Automated Code Reviews

**By**: Alexander Embiricos
**Host**: Claire Vo
**Source**: [How I AI (ChatPRD / Lenny's Podcast Network)](https://www.chatprd.ai/how-i-ai/advanced-codex-workflows-with-openai-alex-embiricos)
**Type**: podcast

## Summary

Four workflows from beginner to advanced. **Workflow 1 (Zero-to-One)**: Use Codex in VS Code to understand unfamiliar codebases (ask "how do I run this?") and make simple changes via natural language (e.g., "jump is way too big, lower please"). Codex identifies relevant code, forms plan, presents diff. **Workflow 2 (Git Worktrees)**: Codex creates worktrees from terminal commands for parallel isolated development — two instances work simultaneously on different branches without merge conflicts. **Workflow 3 (Plans.md)**: Meta-planning technique from OpenAI blog — create a Plans.md template that instructs the model how to structure implementation plans (self-contained milestones, edge cases, updating as it works). Feed task + Plans.md → detailed multi-step plan → review → execute. Used to build Sora Android app in 28 days. Plans can be 120+ lines. **Bonus (Automated Code Review)**: Codex integrated into GitHub PRs — auto-scans changes, flags only high-confidence issues, engineers can reply "fix it" and Codex pushes a commit. Calibrated to protect scarce human attention. Used on almost every OpenAI repo.

## Key Ideas Extracted

- **Engineer as architect/curator, not author**: Role shifts from writing code line-by-line to reviewing, directing, and curating AI-generated work at a higher level of abstraction
- **Plans.md as meta-plan**: Give the model instructions on HOW to plan (structure, milestones, edge cases) rather than just WHAT to build — creates more reliable, reviewable plans
- **Git worktrees + parallel agents = multiplied throughput**: Multiple isolated environments let you prototype conflicting ideas simultaneously without merge conflicts
- **Protect scarce human attention in code review**: Automated reviews should only flag high-confidence issues — false positives waste more human time than they save
- **In-thread fixing closes the loop**: Reply "fix it" to a Codex review comment → new commit pushed — entire review-fix cycle happens in GitHub without switching contexts
- **Codex accessible to non-engineers**: PM or designer can ask "how do I run this?" and make natural-language changes to unfamiliar codebases — lowers the barrier to contribution
- **AI handles "developer toil"**: Complex git commands, boilerplate setup, and tooling configuration — Codex manages these so developers focus on decisions, not mechanics
- **28-day shipping velocity**: Small team built entire Sora Android app using Plans.md technique — structured planning + AI execution enables extreme speed

## Notes

- Published Jan 12, 2026 on ChatPRD blog. 9-min read.
- Tools: Codex (VS Code extension, terminal, GitHub integration), Git worktrees
- Codex included with ChatGPT Plus plan
- Pro-tip: drag Codex icon to VS Code secondary sidebar (right side) for easier access
- Plans.md template available on OpenAI blog
- Sponsors: Brex, Graphite (AI code review platform)
- Cross-reference: Lenny's Newsletter post "Why humans are AI's biggest bottleneck" (same guest)

## Raw Content

*Re-scraped from ChatPRD 2026-02-15. Full article content captured in Summary and Key Ideas above.*
