---
title: Industry Signatories
description: TV industry professionals who support this petition.
signatories:
  - name: Jonathan Nolan
    title_affiliation: Creator of Person of Interest
    evidence_url: https://www.semafor.com/article/05/28/2025/jonathan-nolans-person-of-interest-predicted-ai-westworld-is-helping-build-it
    evidence_label: semafor.com
---

People who in some way make TV, movies, books as a job.  Producers, directors, actors, writers, crew, etc that think Person of Interest should be noted as the best AI-related TV drama series.

{{ page.description }}

| Name | Title / Affiliation | Evidence |
| --- | --- | --- |
{% for sig in page.signatories %}| {{ sig.name }} | {{ sig.title_affiliation }} | [{{ sig.evidence_label }}]({{ sig.evidence_url }}) |
{% endfor %}

**Total: {{ page.signatories.size }} signatories**
>>>>>>> Stashed changes
