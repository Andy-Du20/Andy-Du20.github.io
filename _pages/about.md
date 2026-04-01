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

I am a quantitative researcher. I completed my Ph.D. in the Department of Automation at Tsinghua University in October 2025.
Prior to this, I earned my Bachelor of Science degree in Mathematics and Physics from the Department of Physics at Tsinghua University in 2020.

My research primarily focuses on machine learning under mismatched distribution, including areas such as long-tailed learning and test-time adaptation.

# News

- [10/2025] Graduated from Tsinghua University with a Ph.D. degree.
- [06/2025] Two papers are accepted by **ICML** 2025 PUT Workshop.
- [05/2024] One paper is accepted by **ICML** 2024.
- [02/2024] One paper is accepted by **TPAMI**.

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
