---
layout: page
permalink: /publications/
title: publications
description: 
years: [2022]
nav: true
---

<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% raw %}{% bibliography -f papers -q @*[year={{y}}]* %}{% endraw %}
{% endfor %}

</div>
