---
layout: publication
permalink: /publications/
title: Publications
description: publications
years: [2025, 2024, 2023, 2022]
nav: true
nav_order: 5
---
<!-- _pages/publications.md -->

<p>An up-to-date list is available on <a href="https://scholar.google.com/citations?user=Q40h6VoAAAAJ&hl=en" target="_blank" rel="noopener noreferrer">Google Scholar</a>.</p>

<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f {{ site.scholar.bibliography }} -q @*[year={{y}}]* %}
{% endfor %}

</div>
