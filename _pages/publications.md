---
layout: page
permalink: /Experiences/
title: Work Experience
description: Industrial Affiliations, Work Experience and Responsibilities
years: [2019-Present, 2019-2016, , 2014-2015, 2013-2014]
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
