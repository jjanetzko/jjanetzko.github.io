layout: page
title: pubs
permalink: /pubs/
description: 
years: [2022, 2021, 2020, 2018, 2017, 2016, 2015, 2014, 2013, 2012, 2010, 2008]
nav: true
---

<div class="Publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
