---
created: 2026-02-17
updated: 2026-02-17
template: templates/source.md
template_version: 3
tags: [source, ai-pm]
status: read
source_type: article
source_url: "https://every.to/source-code/how-to-build-agent-native-lessons-from-four-apps"
archive_url: "domains/professional-development/ai-pm/sources/2026-02-17-how-to-build-agent-native-lessons-from-four-apps.md"
author: "Katie Parrott"
published: 2026-02-17
discovered: 2026-02-17
summary: "Four Every apps (Cora, Sparkle, Monologue, Dan Shipper's book-tracking app) demonstrate agent-native architecture: give the AI a minimal toolset (read/write/list) and let it compose behavior rather than coding every feature. Key lessons: simpler/more atomic tools produce smarter emergent behavior; safety constraints belong in the tools themselves not the prompt; retrofitting existing apps is possible via CLI sandboxes and skills-based instruction layers."
domain: professional-development
project: ai-pm
scraped_by: claude
---

# How to Build Agent-native: Lessons From Four Apps

**By**: Katie Parrott
**Source**: [Original URL](https://every.to/source-code/how-to-build-agent-native-lessons-from-four-apps)
**Type**: article

## Summary

A write-up from Every's Agent Native Camp covering how four apps (Dan Shipper's book tracker, Monologue, Cora, Sparkle) are built agent-natively. The core argument: don't code features, define atomic tools and let the AI compose behavior. The most memorable insight is where safety constraints live — not in prompts, but in the tools themselves (Sparkle's delete-with-confirmation lesson).

## Key Ideas Extracted

- **Agent-native architecture** = AI + minimal toolset (read/write/list) → emergent features nobody explicitly programmed; "Claude Code in a trench coat"
- **Atomic tools → smarter composition**: smaller, more single-purpose tools produce more creative AI combinations; the app's feature surface isn't coded, it emerges
- **Safety belongs in tools, not prompts**: Sparkle's Yash learned this after the agent deleted everything in "god mode" — confirmation steps must be baked into the tool, not asked for in the prompt
- **Three principles**: Parity (agent can do anything user can), Granularity (tools are atomic), Composability (emergent behavior from combinations)
- **Retrofitting path**: Cora's Kieran built a CLI sandbox to experiment outside production, then layered in skills (text-based instruction layers) as a middle ground between hardcoded tools and pure prompting
- **Code as scaffolding**: in agent-native dev, you write scaffolding, then rewrite it every ~6 months as model capabilities improve — Anthropic's Claude Code team reportedly works this way already

## Notes

Fits squarely in adjacent disciplines / software dev methodologies. This is less about PM craft and more about how agent-native software is architectured — useful context for understanding what engineers building with AI are actually doing and why.

The "god mode" / Sparkle deletion story is a concrete, memorable illustration of a principle that comes up abstractly everywhere: prompt-level instructions are weak guardrails; architectural constraints (tool-level enforcement) are strong ones. That's directly applicable to how you think about agent risk in product design.

The "code as scaffolding, rewrite every 6 months" framing is worth internalizing — it implies a different relationship to tech debt and longevity than traditional software. Not a bug to manage, but a feature of the paradigm.

The agent-native test ("describe an unanticipated outcome; if the agent can get there from its tools, you've built agent-native") is a clean north-star definition.

## Raw Content

**How to Build Agent-native: Lessons From Four Apps**
*Start with three simple tools, and let the AI figure out the rest*

By Katie Parrott | February 17, 2026 | Source Code

Dan Shipper scanned a page from Erik Larson's biography of Winston Churchill, The Splendid and the Vile, and pressed save. The app he was demo-ing identified the book, grabbed metadata, pulled related content from his existing notes, and surfaced relevant passages. Nobody programmed it to do any of this.

Instead, Dan's app has a handful of basic tools—"read file," "write file," and "search the web"—and an AI that figures out how to use them to fulfill any request.

This is what we call agent-native architecture—or, in Dan's shorthand, "Claude Code in a trench coat." On the surface, it looks like regular software, but underneath, an AI agent is doing the work.

At our first Agent Native Camp, Dan and the general managers of our software products Cora, Sparkle, and Monologue share the key principles they've learned building this way.

**Key takeaways**

- The AI is the app. Instead of coding every feature, you define a few simple tools the AI is allowed to use—for instance, "read file," "write file," and "search the web"—and then let the AI figure out how to combine them.
- Simpler tools get smarter results. The smaller and more basic you make each tool, the more creatively the AI combines them. Claude Code's compound engineering plugin is a good example.
- Rules belong in the tools, not the instructions. You can ask an AI to be careful, but it might ignore you. If an action is irreversible—like deleting a file—build the confirmation step directly into the tool.
- You don't have to start over to start learning. Give the AI a safe space to interact with your existing app and experiment outside the live product.

**How agent-native works**

Traditional software can only do what it's explicitly programmed to do by its code. Click "sort by date" and it sorts by date. Ask it to do something that wasn't coded, and it doesn't know how.

Instead of coded features, an agent-native app has tools (small, discrete actions like "read file" or "send email") and an AI that figures out how to chain those tools together to do whatever the user asks—even if no one anticipated the request.

Three principles make this work:

- Parity: Whatever the user can do, the agent can do. Every click, form submission, and interaction is available as a tool.
- Granularity: Tools should be atomic—small and single-purpose—and features, such as a personalized book summary or a folder deep-clean, emerge from the AI combining them.
- Composability: When tools are atomic and skills can combine them freely, the app develops the ability to do things nobody explicitly programmed.

But there are trade-offs. Agent-native apps are slower because the agent has to reason through each step, and they're more expensive because AI inference costs money. Dan's bet is that inference costs—the price of having the AI think—drop roughly 80 percent every few years, and speed will improve, making the trade-offs increasingly worth it. Cora, built by Kieran Klaassen, is an early example of this approach applied to email.

**Three tools and a filesystem**

Naveen Naidu, general manager of Monologue, took the architecture to its most minimal extreme. He'd been building a read-later app, inspired by Instapaper, where users save articles to read offline.

Web apps typically store data in databases, using structured query languages like SQL to retrieve information. Naveen's approach: ditch the database. Instead, each saved article becomes a file in a folder. The agent has three tools: read a file, write a file, list all files. That's it.

Those simple building blocks determine what the agent—and ultimately the user—can achieve. Ask the agent to "summarize everything I've saved this week" and it lists the files, reads them, and writes a summary—all from three tools.

**When agents go rogue**

When an agent can combine tools on its own, it can also take actions you never intended—including destructive ones. Yash Poojary, general manager of Sparkle, learned this the hard way.

He was working on Deep Clean, a feature to help users clear junk out of their folders. The problem is that "junk" is subjective, and deletion is irreversible.

Yash told agent-native Sparkle, "Keep anything from the last seven days, delete anything older," and went to make coffee. When he came back, the agent had deleted everything—including files he wanted to keep.

The problem emerged when the agent went into what Yash calls "god mode." It started deleting files without asking—because nothing in its toolset required it to ask.

So Yash moved the guardrails from the prompt into the tools themselves. The delete tool now requires explicit confirmation before it can be called. The agent can suggest deletions, but it can't execute them without human approval baked into the tool itself.

**Retrofitting an existing app**

Dan and Naveen's apps were built from scratch. Kieran, on the other hand, has to make Cora, an email assistant with active users, agent-native without breaking anything.

Kieran initially resisted the push toward agent-native. He was thinking about the app's active users and how any transition could disrupt their experience.

His first move was outside the app entirely. He built a command-line interface (CLI)—a text-based way to interact with his app outside of the production environment—to experiment with agent-native flows safely.

Kieran experiments with potential agent-native flows for Cora before he lets them near production.

For example, his experimentation revealed there were too many tools and too much business logic baked into the code. But as Yash's example illustrates, the fix isn't as simple as "move everything into the prompt." Cora needed guardrails.

Kieran's solution has been to lean hard into skills—text-based instructions that split the difference between hardcoded tools and pure prompting.

**Get used to tossing your code every six months**

In traditional software development, code is the product. You build, maintain, and improve it over time.

In agent-native development, code is scaffolding. You write it, the AI builds on it, and then—as AI capabilities improve—you throw it out and rewrite it from scratch, leaning more on the AI each time.

Dan talked with the Anthropic team building Claude Code, and according to them, they work this way already. They write scaffolding to solve problems today and assume they'll rewrite it in six months with better models.

**The agent-native test**

Here's how to know if you've built an agent-native application: Describe an unanticipated outcome to your AI. If it can figure out how to get there from the tools it has, you've built something agent-native.

Every's guide to agent-native architecture breaks down the principles and patterns in detail. And if you want to try it yourself: Open Claude Code or the Codex app with a simple project and give it just three tools. See what it figures out.

These insights emerged from Every's Agent-native Camp, a live workshop where our engineering team shared what they've learned building AI-native software. Register this Friday for our Compound Engineering Camp to learn about the AI-native philosophy that helps Every ship products with single-person teams.
