---
title: "Harness Engineering: Leveraging Codex in an Agent-First World"
created: 2026-02-13
updated: 2026-02-13
template: templates/source.md
template_version: 3
tags: [source, ai-pm, article]
status: unread
source_type: article
source_url: "https://openai.com/index/harness-engineering/"
archive_url: "domains/professional-development/ai-pm/sources/2026-02-13-harness-engineering-leveraging-codex.md"
author: "OpenAI"
published: 2026-02-13
discovered: 2026-02-13
summary: "OpenAI built an internal product with 0 manually-written code using Codex agents over 5 months — 1M lines, 1500 PRs, 3 engineers. Covers agent-first engineering: redefining engineer role, progressive context disclosure, repository as system of record, enforcing architecture mechanically, entropy management."
domain: professional-development
project: ai-pm
---

# Harness Engineering: Leveraging Codex in an Agent-First World

**By**: OpenAI
**Type**: article
**URL**: https://openai.com/index/harness-engineering/

## Summary

OpenAI's team built and shipped an internal product with **0 lines of manually-written code** using Codex agents over 5 months. The product has ~1M lines of code, ~1,500 PRs merged, started with 3 engineers (now 7), averaging 3.5 PRs/engineer/day. Core philosophy: "Humans steer. Agents execute."

Key topics:
- **Redefining the engineer**: Primary job became enabling agents to do useful work — designing environments, specifying intent, building feedback loops
- **Progressive context disclosure**: AGENTS.md as table of contents (~100 lines), not encyclopedia; structured docs/ as system of record
- **Repository as the source of truth**: Anything not in-repo is invisible to agents (Slack convos, Google Docs, tribal knowledge)
- **Agent legibility**: Optimize codebase for agent readability first; favor "boring" composable tech
- **Enforcing architecture mechanically**: Rigid layer model (Types → Config → Repo → Service → Runtime → UI), custom linters, structural tests
- **Entropy/garbage collection**: Recurring cleanup agents scan for drift, open refactoring PRs; "technical debt is a high-interest loan"
- **Increasing autonomy**: Single prompt → reproduce bug → fix → video proof → PR → respond to feedback → merge

## Key Ideas Extracted

*Not yet processed.*

## Notes

- Context from user: "add to ai-pm / horizontal / software development methodologies"
- Particularly relevant to: agent lifecycle management, context management, software delivery methodology
- "Give Codex a map, not a 1,000-page instruction manual" — aligns with home-brain's own CLAUDE.md philosophy
- 6+ hour single agent runs while humans sleep
- Agent-to-agent review replacing human review over time
- Custom linter error messages designed to inject remediation instructions into agent context

---

[← Back to Source Registry]()
