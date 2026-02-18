---
created: 2026-02-17
updated: 2026-02-17
template: templates/source.md
template_version: 3
tags: [source, ai-pm]
status: unread
source_type: article
source_url: "https://every.to/source-code/teach-your-ai-to-think-like-a-senior-engineer-789ba7ca-ca7c-45a1-91fa-4178f59f226f"
archive_url: "domains/professional-development/ai-pm/sources/2026-01-29-teach-your-ai-to-think-like-senior-engineer.md"
author: "Kieran Klaassen"
published: 2026-01-29
discovered: 2026-02-17
summary: "Kieran Klaassen lays out 8 planning strategies for AI-assisted engineering, ordered by complexity: (1) reproduce+document bugs, (2) ground in best practices, (3) ground in your codebase, (4) ground in your libraries, (5) study git history, (6) vibe prototype for clarity, (7) synthesize with options, (8) review with style agents. The insight: running specialized research agents in parallel before coding prevents building wrong solutions — with concrete example of Gmail bulk-archive feature that would have failed without upfront rate-limit discovery."
domain: professional-development
project: ai-pm
scraped_by: claude
---

# Teach Your AI to Think Like a Senior Engineer

**By**: Kieran Klaassen
**Source**: [Original URL](https://every.to/source-code/teach-your-ai-to-think-like-a-senior-engineer-789ba7ca-ca7c-45a1-91fa-4178f59f226f)
**Type**: article

## Summary

*Fill after reading with your own take. 2-3 sentences: what is this about, what's the core argument or insight? (The frontmatter `summary` field has the auto-generated triage summary from ingestion.)*

## Key Ideas Extracted

*Fill during processing. Each idea links to a knowledge entry.*

## Notes

*Your annotations, reactions, questions, disagreements. Written during or after reading.*

## Raw Content

**Teach Your AI to Think Like a Senior Engineer**
*These are the eight strategies I use to help my AI learn my codebase, my patterns, and my preferences*

By Kieran Klaassen | January 29, 2026 | Source Code

I've written about why having your AI coding assistant plan before it codes lets you ship faster than jumping straight to code. It's my method for making my AI smarter with every feature.

For example, when I needed to implement Cora's email bankruptcy feature—clearing 53,000-email inboxes without deleting anything important—I didn't start by coding. I created a research agent to plan instead.

I thought this would be an easy feature. Bulk archive 53,000 emails—how hard could it be? I asked the research agent to analyze our own bulk operation patterns, check API limits for mass actions, and propose three implementation approaches with tradeoffs.

Twenty minutes later, it came back with a reality check: Gmail rate limits would kill us at 2,000 emails, our system would timeout on long operations, and the user would have to wait too long for the result. I thought it would be a quick feature, but it turned into a three-day architectural challenge. Planning had saved me from wasting time building the wrong solution.

**The eight planning strategies**

**Strategy 1: Reproduce and document**
When you encounter a bug, have the AI reproduce it first, document the exact behavior, and only then plan a fix.

**Strategy 2: Ground in best practices**
Before building anything, have the AI research industry best practices for that specific problem.

**Strategy 3: Ground in your codebase**
Have the AI read and understand your existing patterns before writing new code.

**Strategy 4: Ground in your libraries**
Have the AI check the documentation and current versions of your dependencies before using them. (Example: it found a 3-month-old PR showing a library upgrade to v2 put inbox emails in the archive — catching a potential bug before it happened.)

**Strategy 5: Study git history**
Have the AI study the commit history to understand why decisions were made, not just what they were.

**Strategy 6: Vibe prototype for clarity**
When requirements are unclear, build a quick throwaway prototype to explore the problem space before committing to an approach.

**Strategy 7: Synthesize with options**
Have the AI produce multiple implementation options with tradeoffs rather than a single plan.

**Strategy 8: Review with style agents**
After building, use specialized agents to review for code style, performance, security, and other concerns.

**Getting started: Try this today**

Pick your next feature. Before writing any code, create a research agent to analyze the problem. Give it access to your codebase, your libraries' docs, and your git history. Ask it to propose three approaches with tradeoffs. The 20 minutes you spend planning will save hours of rework.
