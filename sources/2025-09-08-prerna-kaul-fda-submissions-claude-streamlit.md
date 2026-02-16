---
title: "How Prerna Kaul Automates 60,000-Page FDA Submissions and Coaches PMs with AI"
created: 2026-02-15
updated: 2026-02-16
template: templates/source.md
template_version: 3
tags: [source, ai-pm, claude-added]
status: unread
source_type: podcast
source_url: "https://www.chatprd.ai/how-i-ai/ai-automate-fda-submissions"
archive_url: ""
author: "Prerna Kaul"
host: "Claire Vo"
published: 2025-07-14
discovered: 2026-02-15
summary: "Prerna Kaul (product/platform leader, Amazon Alexa → Moderna → Panasonic Well) on How I AI. Two workflows tackling technical and human challenges: (1) Automating FDA Biologics License Applications — treated Claude as a co-founder/software engineer, gave it a high-level prompt with problem, business impact, and desired outcome; Claude generated complete project plan (Markdown instructions, capabilities list, demo script, Python code) in minutes vs. a week of traditional planning; built PHI redaction using medical named entity recognition models and RegEx, wrapped in Streamlit UI for non-technical colleagues; generates Common Technical Document (CTD) modules with proprietary XML download; built-in cost analysis feature tracking token costs per operation for transparent ROI and stakeholder buy-in; (2) AI communication coach for stakeholder management — used Anthropic Console Prompt Generator to create structured master prompt for 'Influence and Communication Coach,' uploaded Dale Carnegie and Jane Austen from Project Gutenberg as knowledge base in Claude Projects; generates realistic high-stakes scenarios with competing stakeholders, produces comprehensive strategic playbooks with day-by-day pre-work plans, minute-by-minute meeting agendas, and back-pocket questions for curveballs. Core insight: AI solves both highly technical problems (60,000-page regulatory documents) and deeply human ones (stakeholder alignment), using a pragmatic problem-first approach."
domain: professional-development
project: ai-pm
# taxonomy_inference: horizontal/agents (domain-specific-agents); product-lifecycle/build (feature-specification-writing); horizontal/prompting (communication-coaching)
# provenance: bulk-added by Claude from podcast-episode-compilation.md (2026-02-15)
# rescrape_needed: false — re-scraped from ChatPRD 2026-02-16
---

# How Prerna Kaul Automates 60,000-Page FDA Submissions and Coaches PMs with AI

**By**: Prerna Kaul
**Host**: Claire Vo
**Source**: [How I AI (ChatPRD)](https://www.chatprd.ai/how-i-ai/ai-automate-fda-submissions)
**Type**: podcast

## Summary

How I AI episode with Prerna Kaul, product and platform leader (Amazon Alexa, Moderna, Panasonic Well) working in life sciences where regulatory submissions can reach 60,000 pages. Two workflows solving technical and human challenges: (1) Automating FDA Biologics License Application (BLA) documents — treated Claude as a co-founder and software engineer, gave a high-level prompt with problem description, business impact, and desired outcome; Claude generated a complete project plan in minutes (Markdown instructions, capabilities list, demo narrative script, Python starter code) vs. a week of traditional PM + engineering planning; built PHI (Protected Health Information) redaction using medical named entity recognition models and complex RegEx pattern matching; wrapped everything in a Streamlit UI so non-technical colleagues could generate synthetic clinical data, detect/redact PHI, and produce the Common Technical Document (CTD) with both text and proprietary XML download formats; built-in cost analysis feature tracks token costs and duration per operation for transparent ROI comparisons against manual review; (2) AI-powered communication coach for stakeholder management — used Anthropic Console Prompt Generator to create a structured master prompt for an "Influence and Communication Coach" with XML-like format; uploaded classic literature from Project Gutenberg (Dale Carnegie's "How to Win Friends and Influence People," Jane Austen works, persuasion books) as knowledge base in Claude Projects; generates realistic high-stakes scenarios with competing stakeholders (CEO, Head of Sales, Head of Clinical Data, Chief Legal Officer); produces comprehensive strategic playbooks including situation analysis, tech leader perspectives (Nadella, Jassy), Carnegie communication principles, day-by-day pre-work plans with specific stakeholder conversations, minute-by-minute meeting agendas, and back-pocket answers for curveball questions.

## Key Ideas Extracted

- **Claude as co-founder, not just code assistant**: Treat Claude like a software engineer — explain why the problem matters, the business impact, and desired outcome; it generates complete project plans, not just code snippets
- **PHI redaction without specialized data scientists**: Claude identified correct medical named entity recognition models and generated complex RegEx for pattern matching with minimal domain-specific instruction — work that normally requires months of model development
- **Streamlit for democratizing AI tools**: Wrap Python scripts in Streamlit UI so non-technical colleagues can use sophisticated AI tools directly — runs from terminal with `streamlit run app.py`
- **Built-in cost analysis for stakeholder buy-in**: Track token costs per operation (e.g., PHI redaction cost per patient) and build transparent ROI comparisons directly into the tool — preempts the "AI is too expensive" objection
- **Anthropic Console Prompt Generator**: Use the built-in tool to create sophisticated, structured master prompts with XML-like format — generates better prompts than manual writing for complex coaching scenarios
- **Classic literature as AI knowledge base**: Upload timeless works on persuasion and human dynamics (Carnegie, Austen) from Project Gutenberg to ground communication advice in proven principles
- **Day-by-day strategic playbooks**: AI coach generates not just high-level advice but specific pre-work plans, stakeholder-by-stakeholder conversation guides, minute-by-minute meeting agendas, and prepared answers for anticipated pushback
- **Problem-first approach to AI adoption**: Define the most painful, time-consuming bottleneck first — whether technical (60,000-page documents) or human (stakeholder alignment) — then architect an AI solution around it

## Notes

- Published Jul 14, 2025 on How I AI (ChatPRD). ~9 min read. (Note: filename says 2025-09-08 but actual publication date is Jul 14, 2025)
- Sponsors: CodeRabbit, Lovable
- Prerna Kaul background: Product/platform leader; Amazon Alexa → Moderna → Panasonic Well; works in life sciences/regulatory
- Tools: Claude (planning + coding), Streamlit (UI), Python, Anthropic Console Prompt Generator, Claude Projects, Project Gutenberg (knowledge base source)
- Domain context: Biologics License Application (BLA) — can reach 60,000 pages, 20 specialists, 6 months, millions of dollars
- Key technical details: PHI redaction, medical NER models, RegEx pattern matching, CTD module generation, proprietary XML format
- Two companion workflow guides published Jan 8, 2026
- Cross-references: Regulated industry AI adoption, Claude as co-founder pattern, Streamlit prototyping, AI coaching/mentoring

## Raw Content

*Re-scraped from ChatPRD 2026-02-16. Full article content captured in Summary and Key Ideas above.*
