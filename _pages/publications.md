---
layout: page
permalink: /publications/
title: publications
description: Visit my <a href='https://scholar.google.com/citations?user=JUvNWyYAAAAJ&hl=en&oi=ao'>google scholar page for latest publications. 
years: [2022, 2021, 2020, 2018 ]
nav: true
nav_order: 1
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
