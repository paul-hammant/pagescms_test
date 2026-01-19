---
title: "Petition: Person of Interest - Best AI Series"
description: We believe that Person of Interest is the best AI-related long-story-arc multi-season series in the last 20 years.
signatories: []
---
# We the Undersigned

**{{ page.title }}**

{{ page.description }}

The show's prescient exploration of surveillance, machine learning ethics, and artificial general intelligence remains remarkably relevant today. The philosophical contrast between "The Machine" and "Samaritan" presaged real debates about AI alignment and safety.

## Signature Totals

{% assign industry_page = site.pages | where: "url", "/petition/industry/" | first %}
{% assign journalism_page = site.pages | where: "url", "/petition/journalism/" | first %}
{% assign viewers_page = site.pages | where: "url", "/petition/viewers/" | first %}

{% assign industry_count = industry_page.signatories.size | default: 0 %}
{% assign journalism_count = journalism_page.signatories.size | default: 0 %}
{% assign viewers_count = viewers_page.signatories.size | default: 0 %}
{% assign grand_total = industry_count | plus: journalism_count | plus: viewers_count %}

| Category | Count |
|----------|-------|
| [Industry Professionals](industry/) | {{ industry_count }} |
| [Journalists](journalism/) | {{ journalism_count }} |
| [Viewers](viewers/) | {{ viewers_count }} |
| **Grand Total** | **{{ grand_total }}** |

---

*This petition celebrates a television series that asked important questions about AI before most of us were asking them.*
