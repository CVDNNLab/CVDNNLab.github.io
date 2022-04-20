---
layout: page
permalink: /publications/
title: publications
description: publications by categories in reversed chronological order.
years: [2018, 2017, 2016, 2015, 2014, 2013, 2012, 2011, 2010, 2008, 2007, 2004, 2003]
nav: true
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
