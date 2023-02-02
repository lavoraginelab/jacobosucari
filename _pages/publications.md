---
layout: page
permalink: /publications/
title: publicaciones
description: Publicaciones académicas, libros, artículos y textos.
years: [2022, 2021, 2017, 2018, 2015, 2013, 2011, 2010, 2005, 2004, 2002, 2000, 1999, 1998, 1994, 1993]
nav: true
nav_order: 3
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
