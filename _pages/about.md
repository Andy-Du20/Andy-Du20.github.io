---
permalink: /
title: ""
author_profile: true
redirect_from:
  - /about/
  - /about.html
preprints:
journal_papers: ["ProCo"]
conference_papers: ["SimPro"]
---

# Bio

I am a quantitative researcher now. I completed my Ph.D. in the Department of Automation at Tsinghua University in October 2025.
Prior to this, I earned my Bachelor of Science degree in Mathematics and Physics from the Department of Physics at Tsinghua University in 2020.

My research primarily focuses on machine learning under mismatched distribution, including areas such as long-tailed learning and test-time adaptation.

# Selected Publications


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

<script>
document.querySelectorAll('.archive__item').forEach(item => {
    const titleLink = item.querySelector('.archive__item-title > a');
    const paperLink = item.querySelector('p > a');

    if (titleLink && paperLink) {
        titleLink.href = paperLink.href;
        titleLink.target = '_blank';
        titleLink.rel = 'noopener noreferrer';
    }
});
</script>
