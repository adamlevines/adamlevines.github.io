---
title:  "Publications"
layout: splash
permalink: /publications/
years: [ 2023, 2022, 2021, 2020, 2019, 2018, 2017, 2016, 2015]
nav: true
sort-order: 0
---


<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers.bib -q @*[year={{y}}]* %}
{% endfor %}

</div>
