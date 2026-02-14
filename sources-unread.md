---
layout: default
title: "Sources: Unread"
---

# Unread Sources

Sources captured but not yet read. Sorted by discovery date.

{% assign sources = site.pages | where: "layout", "source" | where: "status", "unread" | sort: "discovered" | reverse %}

{% if sources.size > 0 %}
| Source | Author | Type | Discovered |
|--------|--------|------|------------|
{% for s in sources %}| [{{ s.title }}]({{ s.url }}) | {{ s.author }} | {{ s.source_type }} | {{ s.discovered }} |
{% endfor %}
{% else %}
*All sources have been read!*
{% endif %}
