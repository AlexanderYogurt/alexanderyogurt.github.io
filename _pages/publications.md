---
layout: page
permalink: /publications/
title: publications
description: For a more up-to-date list, please also see my [google scholar](https://scholar.google.com/citations?user=99bFGBsAAAAJ&hl=en&authuser=1) page.  (*=equal contribution)
years: [2022, 2021, 2020, 2019, 2018, 2017]
nav: true
---

<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
