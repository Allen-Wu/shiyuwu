---
layout: page
permalink: /publications/
title: Old publications
description: Pretty old publications back to my undergraduate period.
years: [2019]
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

<hr>
