---
layout: page
permalink: /publications/
title: Publications
description: Full publications on <a href=https://scholar.google.com/citations?user=VIAHsCMAAAAJ&hl=en  style=color:#389AC4>Google Scholar.</a><br> Dagger(†) means equal contribution.
# sections:
#   - bibquery: "@inproceedings"
#     text: "Conferences"
#   - bibquery: "@article"
#     text: "Journals"
years: [2024, 2023]
nav: true
---
<!-- _pages/publications.md -->
<div class="publications">

<!-- {% for section in page.sections %}

  <a id="{{section.text}}"></a>
  <p class="bibtitle">{{section.text}}</p>

  {%- for y in page.years %}
    <h2 class="year">{{y}}</h2>
    {%- bibliography -f papers -q {{section.bibquery}}[year={{y}}] -%}
  {% endfor %}

{% endfor %} -->

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>