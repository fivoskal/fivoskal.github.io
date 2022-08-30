---
layout: page
permalink: /publications/
title: publications
description: publications
nav: true
years: [2021, 2022]
---

<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
