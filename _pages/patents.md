---
layout: page
permalink: /patents/
title: patents
description: Patents in reversed chronological order
years: 
nav: true
nav_order: 1
---
<!-- _pages/publications.md -->
<div class="patents">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
