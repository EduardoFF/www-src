---
#layout: default
title: "Publications"
permalink: /publications/
author_profile: true
years: [2019, 2018, 2017, 2016, 2015, 2014, 2013, 2012, 2011]
---
You can also find my articles on my [Google Scholar profile](https://scholar.google.ch/citations?user=Ov2iGjsAAAAJ&hl=en).

{% for y in page.years %}
  <h3  id="{{y}}" class="pubyear">{{y}}</h3>
  {% bibliography -q @*[year={{y}}]* %}
{% endfor %}
