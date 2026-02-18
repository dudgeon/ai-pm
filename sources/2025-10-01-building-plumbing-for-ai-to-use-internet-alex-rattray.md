---
title: "He's Building the Plumbing For AI to Use the Internet"
created: 2026-02-17
updated: 2026-02-17
template: templates/source.md
template_version: 3
tags: [source, ai-pm, claude-added]
status: unread
source_type: podcast
source_url: "https://every.to/podcast/he-s-building-the-plumbing-for-ai-to-use-the-internet"
archive_url: ""
author: "Alex Rattray"
host: "Rhea Purohit"
published: 2025-10-01
discovered: 2026-02-17
summary: "Alex Rattray (founder, Stainless) explains MCP as native interfaces for language models — like websites for humans, but for AI. Key design principles for MCP servers: limited tool sets (too many options confuse models), clear naming and descriptions, minimal input fields (only essential parameters), streamlined outputs (filter JSON). Hardest problem: designing ergonomic API exposure is harder than building Python SDKs because understanding how LLMs process information is less straightforward. Stainless built a 'shared company brain' using Claude Code — useful insights auto-archived to GitHub."
domain: professional-development
project: ai-pm
---

## Raw Content

# Article Extract: Building the Plumbing for AI to Use the Internet

## Overview
This podcast episode features Alex Rattray, founder of Stainless, discussing Model Context Protocol (MCP)—a new standard enabling AI systems to interact with software tools and APIs.

## Key Concepts

**APIs and MCPs as Internet Infrastructure**
Rattray compares APIs to dendrites in the brain: "APIs are at the heart and center of [modern software], just like dendrites are the center of the mesh of the brain." MCPs represent the next evolution, creating native interfaces for language models similar to how websites present interfaces for humans.

**The Challenge of LLM-Friendly Design**
The fundamental difficulty lies in ergonomic API exposure. As Rattray explains, developing intuitive interfaces for language models proved harder than creating Python SDKs for developers, since understanding how LLMs process information remains less straightforward.

## Design Principles for MCP Servers

Stainless has identified critical patterns:

1. **Limited tool sets** - Too many options confuse models
2. **Clear naming and descriptions** - Precise language guides appropriate usage
3. **Minimal input fields** - Only essential parameters, reducing cognitive load
4. **Streamlined outputs** - JSON filtering removes unnecessary data

## Practical Application at Stainless

The company uses MCP servers for business operations—querying customer databases, cross-referencing HubSpot data, and aggregating Notion notes. They've also built what Rattray calls a "shared company brain" using Claude Code, automatically archiving useful insights in GitHub for team access.
