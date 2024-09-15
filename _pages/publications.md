---
layout: page
permalink: /publications/
# permalink: /
title: Publications
description: 
years: [2023, 2020, 2019]
nav: True
nav_order: 1
---

<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
