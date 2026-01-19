---
title: "Industry Signatories"
description: Tech industry professionals, AI researchers, software engineers, and others working in technology who support this petition.
signatories:
  - name: Example Person
    title_affiliation: AI Researcher at Example Corp
    evidence_url: https://twitter.com/example
    evidence_label: Twitter
---
# Industry Professionals

{{ page.description }}

| Name | Title / Affiliation | Evidence |
| --- | --- | --- |
{% for sig in page.signatories %}| {{ sig.name }} | {{ sig.title_affiliation }} | [{{ sig.evidence_label }}]({{ sig.evidence_url }}) |
{% endfor %}

**Total: {{ page.signatories.size }} signatories**
