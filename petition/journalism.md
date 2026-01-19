---
title: "Journalist Signatories"
description: Writers, critics, and journalists covering technology, entertainment, or AI who support this petition.
signatories:
  - name: Example Journalist
    title_affiliation: Tech Writer at Example Publication
    evidence_url: https://example.com/article
    evidence_label: Article
---
# Journalists

{{ page.description }}

| Name | Title / Affiliation | Evidence |
| --- | --- | --- |
{% for sig in page.signatories %}| {{ sig.name }} | {{ sig.title_affiliation }} | [{{ sig.evidence_label }}]({{ sig.evidence_url }}) |
{% endfor %}

**Total: {{ page.signatories.size }} signatories**
