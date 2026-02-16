---
title: "My 24 Hours with Clawdbot (aka Moltbot)—3 Workflows for a Powerful (and Terrifying) AI Agent"
created: 2026-02-15
updated: 2026-02-15
template: templates/source.md
template_version: 3
tags: [source, ai-pm, claude-added]
status: unread
source_type: podcast
source_url: "https://www.chatprd.ai/how-i-ai/24-hours-with-clawdbot-moltbot-3-workflows-for-ai-agent"
archive_url: ""
author: "Claire Vo"
host: ""
published: 2025-11-24
discovered: 2026-02-15
summary: "Claire Vo solo episode: 24-hour hands-on test of Clawdbot (open-source autonomous AI agent) named 'Polly'. Three workflows tested: (1) Secure setup on dedicated machine with isolated accounts/permissions and Telegram integration, (2) Calendar management as EA — simple tasks worked via workaround (agent creates events on its own calendar and invites you) but complex scheduling failed catastrophically (dates off by one day, flooding calendar with incorrect individual events), (3) Async coding + market research — coding too slow for feedback loops but Reddit research was the standout (voice command → synthesized report delivered to email). Key tensions: permission scope creep, LLMs' inability to handle time/dates reliably, 'acting as you vs. acting for you' distinction."
domain: professional-development
project: ai-pm
# taxonomy_inference: horizontal/agents (autonomous-agents, agent-management, delegation); ai-adoption (trust-and-safety)
# provenance: bulk-added by Claude from podcast-episode-compilation.md (2026-02-15)
# rescrape_needed: false — re-scraped from ChatPRD 2026-02-15
---

# My 24 Hours with Clawdbot (aka Moltbot)—3 Workflows for a Powerful (and Terrifying) AI Agent

**By**: Claire Vo
**Source**: [How I AI (ChatPRD / Lenny's Podcast Network)](https://www.chatprd.ai/how-i-ai/24-hours-with-clawdbot-moltbot-3-workflows-for-ai-agent)
**Type**: podcast

## Summary

Hands-on 24-hour test of Clawdbot, an open-source autonomous agent, with unfiltered assessment. **Setup (Workflow 1)**: ~2 hours of dependency installation (Homebrew, Node, Xcode CLI tools) on a dedicated old MacBook with isolated user account. Connected via Telegram (BotFather API token). Created completely separate digital identity — new Google Workspace email, dedicated 1Password vault. Chose Sonnet 4.5 for safety/cost reasons over Opus. **Calendar EA (Workflow 2)**: Simple single-event scheduling worked via workaround (agent creates on its own calendar, invites you) — but initial OAuth requested all Google scopes when only calendar-read was needed (agent admitted over-requesting when challenged). Complex family calendar scheduling failed badly — every event off by one day, can't create recurring events, and bot tried to re-add events while Claire was deleting them. **Async work (Workflow 3)**: Coding a Next.js conversation viewer worked locally but latency too slow for coding feedback loops. Reddit market research was the star — voice command via Telegram produced excellent structured Markdown report with actionable insights, delivered to email. **Verdict**: Uninstalled after 24 hours due to security concerns. Has category-level product-market fit but isn't ready for non-developers.

## Key Ideas Extracted

- **Question every permission scope**: Agent initially requested all Google scopes (files, contacts, calendar, email) for a calendar-read task — immediately backed down when challenged. Always push back on excessive permissions.
- **Act FOR me, not AS me**: Constant tension between agent impersonating the user vs. working on their behalf — this is a fundamental design challenge for autonomous agents
- **Dedicated machine + isolated accounts**: Security best practice — separate user account, dedicated email, separate password vault with only agent-specific credentials
- **LLMs can't reliably handle time/dates**: Calendar events were consistently off by one day; agent admitted to "mentally calculating" dates instead of using API data — fundamental limitation
- **Research > real-time tasks for agents**: Async research (Reddit scrape → synthesized report) is ideal because latency is a feature, not a bug — matches natural delegation patterns
- **Voice → action → email delivery**: Compelling UX pattern — give voice command via messaging app, receive polished deliverable in inbox
- **Category has PMF, product doesn't**: Clawdbot proved the concept of always-on autonomous agents but the specific implementation is too risky/technical — open question of whether big tech or startups will build the viable version
- **Workaround pattern for trust**: Instead of granting write access to your calendar, have the agent use its own calendar and invite you — pattern applicable to other permission-sensitive domains

## Notes

- Published Jan 28, 2026 on ChatPRD blog. 11-min read. Solo episode.
- Named the Clawdbot instance "Polly"
- Chose Sonnet 4.5 specifically out of fear of what Opus might do autonomously — interesting model selection rationale
- Tools: Clawdbot/Moltbot (open-source agent), Telegram (messaging interface), Google Workspace (email/calendar), 1Password (credential isolation), Anthropic API
- The family calendar disaster is a cautionary tale — deleted events being re-added by the bot while she was on the phone at Target
- Ultimately uninstalled and deleted all keys/tokens after the test
- Sponsor: Lovable

## Raw Content

*Re-scraped from ChatPRD 2026-02-15. Full article content captured in Summary and Key Ideas above.*
