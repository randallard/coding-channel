---
layout: default
title: Journal
nav_order: 3
permalink: /docs/journal/
has_children: true
---

# Great Code with AI Journal

This journal documents the planning, development, and growth of the Great Code with AI YouTube channel. Each entry captures key decisions, challenges faced, and progress made throughout the project.

## Latest Entry

{% assign latest_entry = site.html_pages | where: "parent", "Journal" | sort: "date" | reverse | first %}
{% if latest_entry %}
### [{{ latest_entry.title }}]({{ latest_entry.url | relative_url }})
**Date:** {{ latest_entry.date | date: "%B %d, %Y" }}

{{ latest_entry.content | markdownify | strip_html | truncate: 300 }}

[Read full entry]({{ latest_entry.url | relative_url }}){: .btn .btn-primary .fs-5 .mb-4 .mb-md-0 .mr-2 }
{% else %}
No journal entries have been created yet. Check back soon!
{% endif %}

## All Journal Entries

{% assign entries = site.html_pages | where: "parent", "Journal" | sort: "date" | reverse %}
{% for entry in entries %}
- [{{ entry.title }}]({{ entry.url | relative_url }}) - {{ entry.date | date: "%B %d, %Y" }}
{% endfor %}

## Journal Structure

Each journal entry follows a consistent format:
1. **Current Status**: Overview of where the project stands
2. **Accomplishments**: Key achievements since the last entry
3. **Challenges**: Problems encountered and their resolutions
4. **Decisions**: Important choices made with context and rationale
5. **Next Actions**: Prioritized tasks to complete next

## Tags

Common tags used throughout the journal to categorize entries:

- #planning
- #content-creation
- #channel-strategy
- #equipment-setup
- #branding
- #recording
- #editing
- #community
- #analytics
- #growth-strategy