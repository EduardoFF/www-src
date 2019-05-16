---
layout: default
title: "Publications"
permalink: /publications/
author_profile: true
---


{% for y in page.years %}
  <h3  id="{{y}}" class="pubyear">{{y}}</h3>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

{% bibliography %}
