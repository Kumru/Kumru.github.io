---
layout: page
permalink: /publications/
title: Publications
description: You can find an up-to-date list of my publications on <a href="https://scholar.google.com.tr/citations?user=TzEQjOEAAAAJ&hl=en/" target="_blank">Google Scholar</a>.
years: [2021, 2020, 2019, 2018, 2017, 2016, 2015]
nav: true
---

<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
