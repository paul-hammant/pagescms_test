---
title: "Petition: Person of Interest - Best AI Series"
---
# We the Undersigned

We believe that **Person of Interest** is the best AI-related long-story-arc multi-season series in the last 20 years.

The show's prescient exploration of surveillance, machine learning ethics, and artificial general intelligence remains remarkably relevant today. The philosophical contrast between "The Machine" and "Samaritan" presaged real debates about AI alignment and safety.

## Signature Totals

| Category | Count |
|----------|-------|
| [Industry Professionals](industry/) | {% assign industry_lines = site.pages | where: "url", "/petition/industry/" | first %}{% if industry_lines %}{% assign table_content = industry_lines.content | split: "| ---" | last | split: "##" | first %}{% assign rows = table_content | split: "
" | where_exp: "line", "line contains '|'" %}{{ rows.size }}{% else %}0{% endif %} |
| [Journalists](journalism/) | {% assign journalism_lines = site.pages | where: "url", "/petition/journalism/" | first %}{% if journalism_lines %}{% assign table_content = journalism_lines.content | split: "| ---" | last | split: "##" | first %}{% assign rows = table_content | split: "
" | where_exp: "line", "line contains '|'" %}{{ rows.size }}{% else %}0{% endif %} |
| [Viewers](viewers/) | {% assign viewer_lines = site.pages | where: "url", "/petition/viewers/" | first %}{% if viewer_lines %}{% assign table_content = viewer_lines.content | split: "| ---" | last | split: "##" | first %}{% assign rows = table_content | split: "
" | where_exp: "line", "line contains '|'" %}{{ rows.size }}{% else %}0{% endif %} |

**Grand Total: See individual pages for current counts**

---

*This petition celebrates a television series that asked important questions about AI before most of us were asking them.*
