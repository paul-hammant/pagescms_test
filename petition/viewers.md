---
title: "Viewer Signatories"
description: Fans and viewers who appreciate Person of Interest's thoughtful exploration of AI themes.
signatories:
  - name: Example Viewer
    title_affiliation: Software Developer & PoI Fan
    evidence_url: https://example.com/blog
    evidence_label: Blog Post
---
# Viewers

{{ page.description }}

| Name | Title / Affiliation | Evidence |
| --- | --- | --- |
{% for sig in page.signatories %}| {{ sig.name }} | {{ sig.title_affiliation }} | [{{ sig.evidence_label }}]({{ sig.evidence_url }}) |
{% endfor %}

**Total: {{ page.signatories.size }} signatories**
