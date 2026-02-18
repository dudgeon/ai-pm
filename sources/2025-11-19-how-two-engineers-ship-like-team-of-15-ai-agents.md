---
title: "How Two Engineers Ship Like a Team of 15 With AI Agents"
created: 2026-02-17
updated: 2026-02-17
template: templates/source.md
template_version: 3
tags: [source, ai-pm, claude-added]
status: unread
source_type: podcast
source_url: "https://every.to/podcast/how-two-engineers-ship-like-a-team-of-15-with-ai-agents-7bc186bd-b5ea-40cd-9690-963845203f80"
archive_url: ""
author: "Kieran Klaassen, Nityesh Agarwal"
host: "Rhea Purohit"
published: 2025-11-19
discovered: 2026-02-17
summary: "Kieran Klaassen and Nityesh Agarwal demonstrate shipping 6 features, 5 bug fixes, and 3 infrastructure updates in one week via systematic AI agent workflows. Key tool: a meta-prompt using Anthropic's Prompt Improver that transforms rough feature ideas into detailed GitHub issues with implementation plans. Mental model from Andy Grove's High Output Management: catch issues in the planning phase when stakes are low. Claude Code ranked top tier (clear winner for research, workflows, comprehensive capabilities)."
domain: professional-development
project: ai-pm
---

## Raw Content

# How Two Engineers Ship Like a Team of 15 With AI Agents

## Overview

Engineers Kieran Klaassen and Nityesh Agarwal demonstrate how strategic AI agent workflows enable a small team to achieve outsized productivity. In one week, they shipped six features, five bug fixes, and three infrastructure updates by designing systematic processes where each task compounds the next.

## Key Workflow: Prompt That Writes Prompts

The engineers developed a meta-approach using Anthropic's Prompt Improver to create a custom Claude Code command that transforms rough feature ideas into detailed GitHub issues. Each issue includes:

- Clear problem explanation
- Proposed solution
- Technical implementation details
- Step-by-step execution plan
- Relevant existing code and best practices

"Unlike Cursor, which is made to code," Kieran explains, Claude Code reduces friction for thinking through problems before jumping into execution.

## Critical Mental Model: Fix Problems Early

Drawing from Andy Grove's *High Output Management*, Nityesh emphasizes catching issues during planning phases when stakes remain low. "There are chances that Claude's plan wasn't the direction you wanted to go, and you want to catch that before you ask Claude to go and implement."

This prevents costly rework after code generation begins.

## AI Coding Assistants Ranked

**Top tier:**
- **Claude Code** (clear winner for research, workflows, and comprehensive capabilities)
- **Amp** (praised for ergonomic design)
- **Friday** (opinionated workflows that function well)

**Lower tier:**
- **Windsurf** (rapidly declining without Claude 4 access)
- **GitHub Copilot** (ranked last, though newer agentic features untested)

## Related Tools

The team uses **Monologue**, Every's voice-to-text tool, to eliminate typing friction throughout workflows.
