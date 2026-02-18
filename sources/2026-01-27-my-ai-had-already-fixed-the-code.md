---
created: 2026-02-17
updated: 2026-02-17
template: templates/source.md
template_version: 3
tags: [source, ai-pm]
status: unread
source_type: article
source_url: "https://every.to/source-code/my-ai-had-already-fixed-the-code-before-i-saw-it-f4a29a07-ea95-409f-bcb2-487a970bed4a"
archive_url: "domains/professional-development/ai-pm/sources/2026-01-27-my-ai-had-already-fixed-the-code.md"
author: "Kieran Klaassen"
published: 2026-01-27
discovered: 2026-02-17
summary: "Kieran Klaassen opens with a striking scene: opening GitHub to find Claude Code had already self-reviewed its own PR, citing 3 prior pull requests to justify its variable naming and error-handling choices — without being asked. This defines 'compounding engineering': every bug fix, code review, and PR becomes a permanent lesson the AI applies in the next session. The playbook: encode lessons as rules files, use PR references as institutional memory, and let the AI apprentice to your past decisions."
domain: professional-development
project: ai-pm
scraped_by: claude
---

# My AI Had Already Fixed the Code Before I Saw It

**By**: Kieran Klaassen
**Source**: [Original URL](https://every.to/source-code/my-ai-had-already-fixed-the-code-before-i-saw-it-f4a29a07-ea95-409f-bcb2-487a970bed4a)
**Type**: article

## Summary

*Fill after reading with your own take. 2-3 sentences: what is this about, what's the core argument or insight? (The frontmatter `summary` field has the auto-generated triage summary from ingestion.)*

## Key Ideas Extracted

*Fill during processing. Each idea links to a knowledge entry.*

## Notes

*Your annotations, reactions, questions, disagreements. Written during or after reading.*

## Raw Content

**My AI Had Already Fixed the Code Before I Saw It**
*Compounding engineering turns every pull request, bug fix, and code review into permanent lessons your development tools apply automatically*

By Kieran Klaassen | January 27, 2026 | Source Code

Before I opened my laptop, the code had reviewed itself.

I launched GitHub expecting to dive into my usual routine—flag poorly named variables, trim excessive tests, and suggest simpler ways to handle errors. Instead, I found a few strong comments from Claude Code, the AI that writes and edits in my terminal:

"Changed variable naming to match pattern from PR #234, removed excessive test coverage per feedback on PR #219, added error handling similar to approved approach in PR #241."

In other words, Claude had learned from three prior months of code reviews and applied those lessons without being asked. It had picked up my tastes thoroughly, the way a sharp new teammate would—and with receipts.

It felt like cheating, but it wasn't—it was compounding. Every time we fix something, the system learns. Every time we review something, the system learns. Every time we fail in an avoidable way, the system learns. That's how we build Cora, Every's AI-enabled email assistant.

**The 10-minute investment that pays dividends forever**

After every code review, I spend 10 minutes having Claude summarize what we learned and add it to a rules file in the codebase. These rules become the AI's institutional memory—the equivalent of a senior engineer who's reviewed every PR and knows all the gotchas.

**From terminal to mission control**

The compounding engineering approach transforms the developer's role from "person who writes code" to "person who orchestrates agents and encodes lessons." You spend more time reviewing and encoding, less time writing.

**The compounding engineering playbook**

1. When you fix a bug, have the AI document the root cause and add a rule to prevent it.
2. After every code review, extract the lessons and add them to a rules file.
3. Before starting any new feature, have the AI read the full rules file.
4. Reference PR numbers explicitly in rules so the AI can trace the reasoning.

**Stop coding, start compounding**

The shift from vibe coding to compound engineering is the shift from building features to building systems that build features. Each session, the AI gets a little smarter about how you work. Each review, the system gets a little better at anticipating your feedback. The result: a codebase that improves itself.
