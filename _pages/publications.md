---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---


You will find most, if not all, my publications on [dblp](https://dblp.org/pid/275/3108) or 
[google scholar](https://scholar.google.com/citations?user=bxhpseQAAAAJ). It is probably also the most up-to-date place.

## Selected Papers 

{% include base_path %}

{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %}
