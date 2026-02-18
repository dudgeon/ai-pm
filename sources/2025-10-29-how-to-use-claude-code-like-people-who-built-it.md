---
title: "How to Use Claude Code Like the People Who Built It"
created: 2026-02-17
updated: 2026-02-17
template: templates/source.md
template_version: 3
tags: [source, ai-pm, claude-added]
status: unread
source_type: podcast
source_url: "https://every.to/podcast/how-to-use-claude-code-like-the-people-who-built-it"
archive_url: ""
author: "Cat Wu, Boris Cherny"
host: "Rhea Purohit"
published: 2025-10-29
discovered: 2026-02-17
summary: "Cat Wu and Boris Cherny (Anthropic founding engineers of Claude Code) share best practices: use plan mode for complex tasks (doubles/triples success rate); create shared settings.json for team-wide sensible defaults; use stop hooks to run test suites automatically (model keeps going until done); deploy competitive subagent review (multiple specialized subagents challenge each other's findings — real issues get flagged by all three); some engineers spend $1000+/month on code migrations using parallel subagents. Claude Code originated as an internal Anthropic experiment."
domain: professional-development
project: ai-pm
---

## Raw Content

# How to Use Claude Code Like the People Who Built It

## Overview
This article features an interview with Cat Wu and Boris Cherny, founding engineers of Claude Code at Anthropic, discussing best practices for using the AI coding agent.

## Key Learnings from Anthropic Engineers

**Plan Mode for Complex Tasks**
Rather than attempting one-shot solutions, Cherny recommends using plan mode, which has Claude map out steps beforehand. This "double or triple your chances of success on complex tasks" by establishing alignment before writing code.

**Standardized Team Settings**
Creating a shared `settings.json` file in codebases allows teams to pre-approve routine commands and block risky operations, ensuring "everyone inherits the same sensible defaults" rather than configuring preferences individually.

**Stop Hooks for Task Completion**
Power users implement automated actions triggering when Claude finishes tasks. For example, stop hooks can run test suites and direct Claude to fix failures automatically, allowing "the model to keep going until the thing is done."

**Competitive Subagent Review**
Cherny uses multiple subagents simultaneously—some checking style guidelines, others reviewing project history and flagging bugs. Additional subagents challenge initial findings, ultimately producing "awesome" results that catch real issues while minimizing false alarms.

**Code Migration Efficiency**
Some Anthropic engineers spend over $1,000 monthly on Claude Code for code migrations. The approach involves creating to-do lists and deploying parallel subagents, proving particularly effective for framework switches where verification is straightforward.

## Context
Claude Code emerged from an internal Anthropic experiment and has transformed development workflows at companies like Every, enabling non-technical users and accelerating feature development.
