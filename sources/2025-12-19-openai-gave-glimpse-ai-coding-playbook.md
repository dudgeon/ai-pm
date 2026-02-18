---
title: "OpenAI Gave Us a Glimpse Into Their AI Coding Playbook"
created: 2026-02-17
updated: 2026-02-17
template: templates/source.md
template_version: 3
tags: [source, ai-pm, claude-added]
status: unread
source_type: article
source_url: "https://every.to/source-code/openai-gave-us-a-glimpse-into-their-ai-coding-playbook"
archive_url: ""
author: "Katie Parrott"
published: 2025-12-19
discovered: 2026-02-17
summary: "Four OpenAI engineers built the Android Sora app in 28 days using Codex. Key practices: treat AI as a new hire (every session is onboarding), don't overload context (skills > monolithic instruction files), specialize agents (compose police, tech lead, bug hunter — three narrow reviewers outperform one generalist), filter information ruthlessly (only surface failures). The Sora team used 5B tokens for production — efficiency via compound engineering. Cycling metaphor: 'it doesn't get easier, you just go faster.'"
domain: professional-development
project: ai-pm
---

## Raw Content

# OpenAI's AI Coding Playbook: Key Lessons from Building Sora

## Overview
Four OpenAI engineers built the Android version of Sora in 28 days using Codex, their AI coding agent. One engineer, RJ Marsan, injured his wrist during development and adapted by using speech-to-text with Codex—a constraint that revealed crucial insights about effective human-AI collaboration.

## Core Principles

**1. Treat AI as a New Hire**
Rather than viewing Codex as a tool, the team discovered better results treating it like an onboarding colleague. As Marsan noted, "Every session is onboarding this new coworker [anew]." Start with quick, interactive prompts to build trust before delegating longer tasks.

**2. Don't Overload Context**
Codex performs worse when given massive instruction files. Alexander Embiricos stated: "No one needs to know every single fact." OpenAI is shifting toward "skills"—smaller, atomic units of instruction that provide only what's needed for specific tasks.

**3. Specialize Your Agents**
The team created three focused AI reviewers for code review:
- **Compose police**: UI consistency checks
- **Tech lead**: Architectural problems
- **Bug hunter**: Logic errors and edge cases

Narrow specialization outperforms generalist agents. When all three flagged the same code line, developers knew something was genuinely wrong.

**4. Filter Information Ruthlessly**
Showing Codex thousands of routine status updates degraded performance. Filtering to surface only failures dramatically improved output quality—applicable to human reviewers too.

## When to Use Codex

Optimal entry points include:
- Unsolved bugs requiring deep investigation
- Architecture planning and code structure
- Code reviews (via CLI command or GitHub Actions)

The Sora team used 5 billion tokens for their production app—surprisingly efficient according to Embiricos.

## The Reality Check

Marsan offered this cycling metaphor: "It doesn't get easier, you just go faster." AI tools shift bottlenecks rather than eliminate them. Good architecture remains foundational; developers must think about structural decisions *more* often, not less.
