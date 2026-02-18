---
created: 2026-02-17
updated: 2026-02-17
template: templates/source.md
template_version: 3
tags: [source, ai-pm]
status: unread
source_type: article
source_url: "https://every.to/playtesting/we-trained-an-ai-on-a-board-game-it-became-a-better-customer-support-agent-299b5938-09dd-4881-803f-aea21f0d461f"
archive_url: "domains/professional-development/ai-pm/sources/2026-02-03-board-game-training-customer-support-agent.md"
author: "Alex Duffy"
published: 2026-02-03
discovered: 2026-02-17
summary: "Good Start Labs fine-tuned Qwen3-235B on Diplomacy (a board game requiring negotiation and deception) and found it significantly improved on customer support benchmarks — demonstrating that game-based RL training produces generalizable skills. Key claims: games are ideal training environments because they clearly score success; game data is proprietary and dynamic unlike web text; skills like 'reading between the lines' transfer across domains."
domain: professional-development
project: ai-pm
scraped_by: claude
---

# We Trained an AI on a Board Game. It Became a Better Customer Support Agent.

**By**: Alex Duffy
**Source**: [Original URL](https://every.to/playtesting/we-trained-an-ai-on-a-board-game-it-became-a-better-customer-support-agent-299b5938-09dd-4881-803f-aea21f0d461f)
**Type**: article

## Summary

*Fill after reading with your own take. 2-3 sentences: what is this about, what's the core argument or insight? (The frontmatter `summary` field has the auto-generated triage summary from ingestion.)*

## Key Ideas Extracted

*Fill during processing. Each idea links to a knowledge entry.*

## Notes

*Your annotations, reactions, questions, disagreements. Written during or after reading.*

## Raw Content

**We Trained an AI on a Board Game. It Became a Better Customer Support Agent.**
*Games teach transferable skills—to humans and AI alike*

By Alex Duffy | February 3, 2026 | Playtesting

It's my job to make AI play games. One board game we've focused on at Good Start Labs has been Diplomacy, a World War I simulation. John F. Kennedy and Henry Kissinger were fans.

When we fine-tuned the Qwen3-235B model—an open-source model developed by the team at Chinese cloud giant Alibaba—on Diplomacy using reinforcement learning, it improved significantly on a customer support benchmark (TAU-bench) and on AssetOpsBench, a financial operations assessment.

It's not a big leap to believe that improvement in one game could boost the model's performance on other tasks. Humans who are great at one game usually become great at other games. StarCraft players often report that the game taught them to cook efficiently—keeping an eye on multiple processes simultaneously, adapting quickly.

**The game is the curriculum**

"You become good at whatever the system rewards," Every's AI & I producer Rachel Braun tells me. Diplomacy rewards reading between the lines and distinguishing genuine cooperation from strategic manipulation. That kind of nuanced reading transfers to customer support.

It's also why Arcee, a U.S.-based AI lab, is using our Diplomacy environment to fine-tune Trinity Large. What Arcee and other labs are betting on is a second additional way to improve AI—not by making models bigger or feeding them more text, but by putting them in environments where skills can be practiced and measured.

As AI researcher Andrej Karpathy put it: By training models in multiple games and tasks where you can score success, what are you building toward? Not just a game-player, but a general problem-solver.

**The game is also the exam**

Games don't just train models; they generate data no one else has. Our AI agents have played hundreds of thousands of games — Bad Cards included — creating a proprietary dataset.

What users want from AI shifts faster than tests can measure, so static benchmarks become outdated quickly. Games are a natural fit for continuous evaluation. They generate large amounts of data about real decision-making, and the feedback loop is immediate and unambiguous.

**From StarCraft to the frying pan**

Willie didn't set out to learn cooking from StarCraft—he was trying to win. But the skills he learned showed up in the kitchen. AI development is exhibiting the same pattern. If you set a clear goal, the skills to reach it will transfer. Only people can define what those goals should be: what counts as a good decision, what's funny, and what's not.
