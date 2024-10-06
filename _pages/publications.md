---
layout: page
permalink: /publications/
title: Publications
description: 
years: [2024,2023]
nav: true
nav_order: 1
---
<!-- _pages/publications.md -->

An overview of publications based or presented at the workshop. The links if available are to the official/published version, but you should always be able to find a preprint on arXiV as well. 

<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
