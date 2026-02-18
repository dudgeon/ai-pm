---
created: 2026-02-17
updated: 2026-02-17
template: templates/source.md
template_version: 3
tags: [source, ai-pm]
status: unread
source_type: article
source_url: "https://every.to/source-code/stop-coding-and-start-planning-be0b4fd1-5898-4b09-bfda-0b00ea0004fd"
archive_url: "domains/professional-development/ai-pm/sources/2026-01-28-stop-coding-and-start-planning.md"
author: "Kieran Klaassen"
published: 2026-01-28
discovered: 2026-02-17
summary: "Kieran Klaassen argues that vibe coding killed planning and that's a problem — 10 minutes of AI-assisted planning prevents 3 hours of debugging. Plans teach the AI how you think; code just solves problems. Three planning fidelities: (1) quick fix for simple bugs, (2) sweet spot for most features, (3) big uncertain for major architectural decisions. Key insight: unlike code, plans accumulate into the AI's understanding of your codebase, compounding with each feature."
domain: professional-development
project: ai-pm
scraped_by: claude
---

# Stop Coding and Start Planning

**By**: Kieran Klaassen
**Source**: [Original URL](https://every.to/source-code/stop-coding-and-start-planning-be0b4fd1-5898-4b09-bfda-0b00ea0004fd)
**Type**: article

## Summary

*Fill after reading with your own take. 2-3 sentences: what is this about, what's the core argument or insight? (The frontmatter `summary` field has the auto-generated triage summary from ingestion.)*

## Key Ideas Extracted

*Fill during processing. Each idea links to a knowledge entry.*

## Notes

*Your annotations, reactions, questions, disagreements. Written during or after reading.*

## Raw Content

**Stop Coding and Start Planning**
*Spend an hour teaching AI how you think, and it gets smarter with every feature you build*

By Kieran Klaassen | January 28, 2026 | Source Code

AI made us sloppy because it made us forget how to plan.

Planning used to be a non-negotiable part of the work: sketching screens, prototyping flows, and writing problem statements. You had to define the scope—what's in, what's out, what's too ambitious, and what solves the problem. Good planning required good thinking, good writing, and collaboration between stakeholders. It was slow, but it prevented expensive mistakes.

When vibe coding emerged, planning went out the window—at first. Why spend an hour planning when you could spend five minutes building the feature? I did it, too. "Make this feature work" was my entire instruction. Sometimes it worked. Often it didn't. When it didn't, I'd spend three hours debugging an error that a 10-minute session—asking AI to create a clear outline of the problem and the research needed to build a solution—would have prevented. And I'd be starting from zero with each feature I shipped, instead of the AI improving with each request.

When you vibe code, you're not just writing code—you're missing an opportunity to teach your AI how you think. Plans teach the system; code just solves problems.

**How to plan effectively: Remember the three fidelities**

**Fidelity One: The quick fix**
For simple bugs or straightforward tasks, a quick description is enough: "Fix the bug where X happens when Y." These take minutes and prevent the AI from going off in the wrong direction.

**Fidelity Two: The sweet spot**
For most features, a 10-20 minute planning session pays off. Ask the AI to research the problem, identify potential approaches, and recommend one with tradeoffs. This is where most of the value is.

**Fidelity Three: The big uncertain**
For major architectural decisions or features with significant unknowns, invest 1-2 hours of planning. Run multiple specialized research agents in parallel. The upfront cost is worth it.

**How planning creates lasting knowledge**

Unlike code, plans accumulate. Each plan you create with your AI becomes part of the shared understanding it brings to the next feature. When you plan well, you're not just building a feature—you're teaching the AI how you think about problems, what tradeoffs matter to you, and how your codebase works. That knowledge compounds over time.
