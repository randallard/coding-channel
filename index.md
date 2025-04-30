---
layout: home
title: Home
nav_order: 1
permalink: /
---

# Great Code with AI YouTube Channel Documentation

Welcome to the documentation for the Great Code with AI YouTube channel, showcasing how AI can enhance coding productivity and everyday life.

## What is Great Code with AI?

Great Code with AI is a YouTube channel focused on demonstrating practical applications of AI tools for coding, productivity, and learning. Through regular content updates, we explore how AI can solve real programming challenges, assist in long-term projects, and help beginners learn to code.

## About This Project

This channel features:
- Real-world programming tasks solved with AI assistance
- Documentation of a long-term project built with AI
- Beginner-friendly coding tutorials leveraging AI tools
- Practical demonstrations of productivity enhancements

## Project Status
{: .fs-5 }

Want to know where we are in development? Check our [Project Plan & Status]({{ '/docs/project-plan-and-status' | relative_url }}) page to see our current progress, upcoming milestones, and development roadmap.

[View Project Status]({{ '/docs/project-plan-and-status' | relative_url }}){: .btn .btn-primary .fs-5 .mb-4 .mb-md-0 .mr-2 }

## Latest Journal Update
{: .fs-5 }

{% assign latest_entry = site.html_pages | where: "parent", "Journal" | sort: "date" | reverse | first %}
{% if latest_entry %}
### [{{ latest_entry.title }}]({{ latest_entry.url | relative_url }})
**Date:** {{ latest_entry.date | date: "%B %d, %Y" }}

{{ latest_entry.excerpt | truncate: 150 }}

[View latest update]({{ latest_entry.url | relative_url }}){: .btn .btn-primary .fs-5 .mb-4 .mb-md-0 .mr-2 }
[Journal]({{ '/docs/journal' | relative_url }}){: .btn .fs-5 .mb-4 .mb-md-0 .mr-2 }
{% else %}
Journal entries coming soon!

[Journal]({{ '/docs/journal' | relative_url }}){: .btn .fs-5 .mb-4 .mb-md-0 .mr-2 }
{% endif %}

## Content Categories

Explore our three main content series:

1. **Real-Work Programming Tasks with AI** - Solving authentic coding challenges
2. **Long-Term Project with AI** - Building a complex project from start to finish
3. **Learning to Code from Square 1 with AI** - Beginning coding with AI assistance

[View Content Categories]({{ '/docs/content-categories' | relative_url }}){: .btn .fs-5 .mb-4 .mb-md-0 .mr-2 }