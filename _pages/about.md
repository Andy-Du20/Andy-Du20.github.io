---
permalink: /
title: ""
author_profile: true
redirect_from:
  - /about/
  - /about.html
preprints:
journal_papers: ["ProCo", "HSP"]
conference_papers: ["SwiTTA", "UniTTA", "SimPro", "RISA"]
---

# Bio

I am a quantitative researcher with a Ph.D. in Automation from Tsinghua University (2025). Prior to this, I earned my B.S. in Mathematics and Physics from Tsinghua University (2020).

My research focuses on machine learning under distribution mismatch, including long-tailed learning and test-time adaptation.

# News

- **[10/2025]** Ph.D. graduated from Tsinghua University.
- **[06/2025]** Two papers accepted at **ICML** 2025 PUT Workshop.
- **[05/2024]** One paper accepted at **ICML** 2024.
- **[02/2024]** One paper accepted by **TPAMI**.

# Selected Publications

## Preprints

{% for item in page.preprints %}
{% assign post = site.publications | where: "name", item | first %}
{% include archive-single.html %}

---

{% endfor %}

## Journal Papers

{% for item in page.journal_papers %}
{% assign post = site.publications | where: "name", item | first %}
{% include archive-single.html %}

---

{% endfor %}

## Conference Papers

{% for item in page.conference_papers %}
{% assign post = site.publications | where: "name", item | first %}
{% include archive-single.html %}

---

{% endfor %}
