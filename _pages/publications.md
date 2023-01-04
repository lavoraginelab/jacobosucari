---
layout: page
permalink: /publications/
title: publicaciones
description: Publicaciones en orden cronológico. generadas por jekyll-scholar.
years: [2013, 2015, 2017, 1935, 1905]
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
