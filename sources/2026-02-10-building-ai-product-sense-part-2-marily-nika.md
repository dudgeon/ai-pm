---
title: "Building AI Product Sense, Part 2 | Marily Nika"
created: 2026-02-15
updated: 2026-02-16
template: templates/source.md
template_version: 3
tags: [source, ai-pm, claude-added]
status: unread
source_type: newsletter
source_url: "https://www.lennysnewsletter.com/p/building-ai-product-sense-part-2"
archive_url: ""
author: "Marily Nika"
host: ""
published: 2026-02-10
discovered: 2026-02-15
summary: "Marily Nika (Gen AI Product Lead @ Google, formerly Meta; PhD in ML; AI Product Academy founder) guest post Part 2 on Lenny's Newsletter. Defines AI product sense as 'the ability to translate probabilistic model behavior into a product experience people can rely on.' Meta added 'Product Sense with AI' interview — first major PM loop change in 5+ years — where candidates work through product problems with AI in real time, evaluated on how they handle uncertainty. Provides a concrete weekly ritual system (~15 min/week): Ritual 1 — ask model to do something obviously wrong to surface hallucination patterns (models confidently invent structure from chaos); Ritual 2 — test ambiguous prompts to find semantic fragility; Ritual 3 — give unexpectedly difficult tasks to find first failure point. Introduces Minimum Viable Quality (MVQ) framework with three thresholds: acceptable bar, delight bar, do-not-ship bar — plus cost envelope estimation. Four guardrail design patterns: ask instead of guess when unsure, give user a choice when context too long, say so when inventing structure, add light structure when outputs bounce. Real example: AI Slack thread summarizer was assigning owners when no one volunteered — single system prompt constraint eliminated the trust issue. Core insight: 'fix the model' is usually the wrong answer — 'decide what the product does when the model hits its limits' is right."
domain: professional-development
project: ai-pm
# taxonomy_inference: ai-adoption (role-evolution, skill-development); product-lifecycle/discover (problem-signal-detection)
# provenance: bulk-added by Claude from podcast-episode-compilation.md (2026-02-15)
# rescrape_needed: false — re-scraped via Chrome MCP 2026-02-16
---

# Building AI Product Sense, Part 2 | Marily Nika

**By**: Marily Nika
**Source**: [Lenny's Newsletter / Lenny's Podcast](https://www.lennysnewsletter.com/p/building-ai-product-sense-part-2)
**Type**: newsletter

## Summary

Marily Nika guest post Part 2 on Lenny's Newsletter — a practical guide to building AI product sense through weekly rituals. Meta recently added a "Product Sense with AI" interview, the first major change to its PM interview loop in over five years, where candidates work through product problems with AI in real time and are evaluated on how they handle uncertainty (not prompting tricks or model trivia). AI product sense is defined as the ability to translate probabilistic model behavior into a product experience people can rely on. Three weekly rituals (~15 min total): **Ritual 1** (2 min) — Ask model to do something obviously wrong to surface hallucination patterns; models confidently invent structure from chaos (e.g., turning an ambiguous Slack thread into a confident but completely wrong roadmap). Compare hallucinated output with corrected output to understand what guardrails fix the failure. **Ritual 2** (3 min) — Test ambiguous prompts to find semantic fragility; model technically understands words but misses intent (e.g., "summarize for execs" returns emoji bullet lists). **Ritual 3** (3 min) — Give unexpectedly difficult tasks to find first failure point; where the model breaks first is where you need design guardrails. Introduces **Minimum Viable Quality (MVQ)** framework with three thresholds: acceptable bar (good enough for real users), delight bar (feels magical), and do-not-ship bar (unacceptable failure rates that break trust). Includes cost envelope estimation — ballpark what the feature costs per user per month at scale. Real-world example from speech recognition: >90% accuracy in controlled tests, completely fell apart with barking dogs, dishwashers, and cross-room speaking. **Ritual 4** — Design guardrails where behavior breaks. Four patterns: (1) when unsure, ask instead of guess; (2) when context too long, give user a choice; (3) when inventing structure, say so; (4) when outputs bounce around, add light structure. Real example: AI Slack summarizer was assigning owners when no one volunteered — a single system prompt constraint eliminated the trust issue. Core insight: "fix the model" is usually wrong; "decide what the product does when the model hits its limits" is right.

## Key Ideas Extracted

- **AI product sense as core PM skill**: The ability to translate probabilistic model behavior into a product experience people can rely on — Meta's new PM interview evaluates exactly this
- **Weekly ritual system for building AI product sense**: Four rituals in ~15 min/week that surface issues before production: test wrong, test ambiguous, test difficult, design guardrails
- **Models confidently invent structure from chaos**: When confronted with mess, generative models hallucinate roadmaps, assign wrong owners, and turn offhand comments into commitments — this is the most dangerous failure pattern
- **Minimum Viable Quality (MVQ) framework**: Three thresholds — acceptable bar, delight bar, do-not-ship bar — defined before development, checked throughout; includes cost envelope estimation
- **Guardrail design > model improvement**: "Fix the model" is usually the wrong answer; deciding what the product does when the model hits its limits is the real product work
- **Four guardrail patterns**: Ask instead of guess when unsure; give user choice when context too long; be transparent when inventing structure; add light structure when outputs bounce
- **Cost envelope as product sense**: If a feature costs $0.30/user/month and drives retention, it's a no-brainer; if $5/user/month with unclear impact, it's a business problem — estimating this early is core AI PM work
- **Semantic fragility**: Models technically understand words but miss intent — ambiguous inputs are kryptonite for probabilistic systems; product design must reduce ambiguity before it reaches the model
- **Lab accuracy vs. production accuracy**: Performance almost always drops in the real world — speech recognition went from >90% in tests to broken with barking dogs and dishwashers
- **Product problem vs. model limitation**: Building AI product sense means you stop being surprised by model behavior and gain clarity on what's a product design issue vs. what's a fundamental model constraint
- **Five strategic context factors for MVQ thresholds**: The specific acceptable/delight/do-not-ship bars aren't fixed — they depend on strategic context factors that raise or lower where you set them
- **AI product sense is converging but not yet defined**: When polled, PMs describe it variously as model knowledge, evaluation, prompting, safety, or cost/unit economics — the industry is still converging on what "great" looks like

## Notes

- Published Feb 10, 2026 on Lenny's Newsletter. Subscriber-only guest post. Also available as podcast (Spotify/Apple/YouTube).
- Marily Nika byline: Gen AI Product Lead @ Google (previously Meta Reality Labs); Fortune 40 under 40
- This is Part 2 — Part 1 exists but is not in our sources yet
- Courses: AI PM Bootcamp & Certification, AI Product Sense and AI PM Interview prep (15% off via article links)
- Real-world examples from shipping speech recognition and speaker identification features for conversational platforms and on-device assistants (10 years experience)
- Cross-reference: Three other Marily Nika episodes in sources — `2023-02-05`, `2024-07-09` (how close AI replacing PMs), `2024-08-13` (summary of 2023 episode)
- Highly actionable — the ritual system and MVQ framework are directly implementable
- Sponsors: Lovable, Manus, Replit, Gamma, n8n, Canva, ElevenLabs, Amp, Factory, Devin, Bolt, and many more offered free to subscribers

## Raw Content

*Re-scraped via Chrome MCP from subscriber tab 2026-02-16. Structured notes below; full text available at source URL (Lenny's Newsletter, subscriber-only).*

### Article Structure

**Introduction**: Meta recently added "Product Sense with AI" to its PM interview loop — the first major change in 5+ years. Candidates work through a product problem with AI in real time. They're evaluated on how they handle uncertainty: noticing when the model is guessing, asking the right follow-ups, making product decisions despite imperfect information. This reflects a broader shift: AI product sense is the new core PM skill.

The uncomfortable truth: the hardest part of AI product development comes when real users arrive with messy inputs, unclear intent, and zero patience. A customer support agent can feel incredible in a demo, then quietly lose trust by confidently answering ambiguous questions instead of stopping to ask for clarification.

Author's three-step process: (1) Map the failure modes, (2) Define the minimum viable quality (MVQ), (3) Design guardrails where behavior breaks.

---

### Step 1: Map the Failure Modes (and the Intended Behavior)

Every AI feature has a "failure signature" — the pattern of breakdowns it reliably falls into when the world gets messy. Fastest way to build AI product sense is to deliberately push the model into those failure modes before users do.

**Ritual 1 — Ask a model to do something obviously wrong (2 min)**
Goal: Understand the model's tendency to force structure onto chaos.

Example: Take a messy Slack thread (half-formed, emotionally inconsistent) and ask the model to extract "strategic decisions." The model's most dangerous pattern: when confronted with mess, it confidently invents structure. It hallucinated a roadmap, assigned wrong owners, turned offhand comments into commitments — looks authoritative, clean, structured, and is completely wrong.

Process after getting wrong results:
1. Re-run the same Slack thread and ask it to draft a Q4 roadmap — observe the hallucination
2. Tell the model what good looks like: "Only include items explicitly mentioned. If something is missing, say 'Not enough information.'" Run again
3. Compare the two outputs side by side — confident hallucination vs. humble clarity. This contrast sharpens AI product sense fastest
4. Capture gaps — these become product requirements. What changed? What guardrail fixed the hallucination? What does the model need to behave reliably?

**Ritual 2 — Ask a model to do something ambiguous (3 min)**
Goal: Understand the model's semantic fragility.

Ambiguity is kryptonite for probabilistic systems. If a model doesn't fully understand intent, it fills gaps with best guesses (hallucinations, bad ideas). That's when user trust cracks.

Practical example: Input a PRD into NotebookLM and ask it to "Summarize this PRD for the VP of Product." Observe: does it over-summarize? Latch onto irrelevant details? Ignore caveats? Assume the wrong audience?

Other examples: ask for a summary for leaders and get emoji bullet lists; ask for UX problems and get a pricing model proposal.

The failures reveal where communication breaks. Product should step in: ask user to choose a goal ("Summarize for who?"), give model more context, or constrain the action. Not trying to trick the model — trying to understand where misunderstandings occur so you can prevent them through design.

Article includes a table of ambiguous prompts to test, what breaks, and what to do about it.

**Ritual 3 — Ask a model to do something unexpectedly difficult (3 min)**
Goal: Understand the model's first point of failure.

Pick one task that feels simple to a human PM but stresses a model's reasoning, context, or judgment. Not exhaustive testing — just finding where it breaks first, which is where the product needs structure.

Example 1: "Group these 40 bugs into themes and propose a roadmap."
Example 2: "Summarize this PRD and flag risks for leadership."

Over time, this also surfaces second-order effects — moments where small AI features quietly reshape workflows, defaults, or expectations.

---

### Step 2: Define Minimum Viable Quality (MVQ)

Performance almost always drops once AI features leave the controlled development environment. Since you don't know how or by how much, define MVQ and check it throughout development.

**Three thresholds:**
- **Acceptable bar**: Good enough for real users
- **Delight bar**: Feels magical
- **Do-not-ship bar**: Unacceptable failure rates that break trust

**Concrete example — Speech recognition/speaker identification:**
Firsthand experience: demos hit >90% accuracy in controlled tests, then completely fell apart in a real home — barking dog, running dishwasher, someone speaking from across the room.

Speaker identification MVQ:
- *Acceptable*: Correctly identifies speaker x% of the time in typical home conditions; recovers gracefully when unsure ("I'm not sure who's speaking—should I use your profile or continue as a guest?")
- *Delight*: Users stop repeating themselves; "No, I meant..." corrections drop sharply. Rule of thumb: 8-9 out of 10 attempts work without retry = feels magical; 1 in 5 needs retry = trust erodes fast. MVQ also depends on phase (closed beta vs. broad launch)
- *Delight tests*: Background chaos test (video playing, two people talking over each other); 6pm kitchen test (dishwasher, kids, dog barking); mid-command correction test ("Set timer for 10 minutes... actually, make it 5")
- *Do-not-ship*: Misidentifies speaker >y% of the time in critical flows (purchases, messages, personalized actions); forces users to repeat themselves multiple times

**Five strategic context factors** that raise or lower the MVQ bar — determines where thresholds should be set (article includes a table/visual for these).

**Cost envelope estimation:**
One of the most common mistakes new AI PMs make: falling in love with a magical demo without checking financial viability.

Cost envelope = rough range of what feature costs to run at scale per user.

Starting questions: Model cost per call? Frequency per user/day/month? Worst-case power users? Can caching/smaller models/distillation reduce costs? If usage 10x's, does the math still work?

Example — AI meeting notes:
- Per-call: ~$0.02 for 30-minute transcript
- Average: 20 meetings/user/month → ~$0.40/month/user
- Heavy users: 100 meetings/month → ~$2.00/month/user
- With caching + smaller model for low-stakes meetings: ~$0.25–$0.30/month/user average
- $0.30/user/month that drives retention = no-brainer; $5/user/month with unclear impact = business problem

---

### Step 3: Design Guardrails Where Behavior Breaks

Guardrails determine what the product does when the model hits its limits. They protect users from experiencing failure modes.

**Real example — AI Slack thread summarizer:** Built to increase team productivity by summarizing Slack threads into "decisions and action items." In testing, worked well — until it started assigning owners for action items when no one had agreed to anything. Sometimes picked the wrong person. Fix was not a different model, but a new guardrail: one line added to system prompt — "Only assign an owner if someone explicitly volunteers or is directly asked and confirms. Otherwise, surface themes and ask the user what to do next." Single constraint eliminated the biggest trust issue almost immediately.

None of the guardrails make the model more intelligent. They protect the user from the model's shortcomings and prevent misunderstandings.

**Ritual 4 — Add explicit failure responses in the system prompt (3 min)**
Take real messy input, feed it in multiple times, ask the same question each time. Compare answers side by side. Look for: did it pick different decisions each time? Invent decisions? Miss the same important decision repeatedly? If user saw worst version, would they still trust the product?

**Four patterns covering most real-world cases:**
1. **When model seems unsure → ask instead of guessing**: Add instruction: "If not confident, ask a clarifying question instead of assuming." Small questions prevent big mistakes downstream
2. **When context is too long → give user a choice**: "This thread is long—should I focus on the first half, second half, or just action items?" Fast, honest, avoids hallucinations
3. **When model invents structure → say so**: "I didn't see any decisions here—would you like themes instead?" Transparency builds trust
4. **When outputs bounce around → add light structure**: Steady with simple format: "List: what was discussed, what was decided, what needs follow-up." Reduces variance without rigidity

---

### Conclusion

AI product sense is a muscle built through repetition. When author polled bootcamp students and PM peers on what it means, answers varied (model knowledge, evaluation, prompting, safety, cost/unit economics). The industry is still converging.

Practical definition: AI product sense is the ability to translate probabilistic model behavior into a product experience people can rely on.

Run rituals once a week → stop being surprised by weird outputs, design clearer asks, tighter constraints, better fallbacks. In 2026, the differentiator will be PMs who ship products that feel trustworthy despite messy inputs, unclear intent, and zero patience.
