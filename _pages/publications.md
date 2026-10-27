---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
excerpt: "Publications and preprints on formal verification, logic, and neural networks."
---

Selected publications and preprints are listed below, newest first. For a full bibliography, see
[DBLP](https://dblp.org/pid/275/3108) or
[Google Scholar](https://scholar.google.com/citations?user=bxhpseQAAAAJ&sortby=pubdate).

{% include base_path %}

## Preprints

{% assign sorted_publications = site.publications | sort: 'date' | reverse %}
{% for post in sorted_publications %}
  {% if post.publication_kind == 'preprint' %}
    {% include archive-single.html %}
  {% endif %}
{% endfor %}

## Selected publications

{% assign publication_year = '' %}
{% for post in sorted_publications %}
  {% unless post.publication_kind == 'preprint' %}
  {% assign year = post.date | date: '%Y' %}
  {% if year != publication_year %}
<h2 class="archive__subtitle">{{ year }}</h2>
    {% assign publication_year = year %}
  {% endif %}
  {% include archive-single.html %}
  {% endunless %}
{% endfor %}

## Edited proceedings

**Marco Sälzer, François Schwarzentruber, and Nicolas Troquard (eds.).**
[Proceedings of the Workshop on Logical Methods for Neural Network Analysis (LOGICNN 2026)](https://ceur-ws.org/Vol-4276/).
CEUR Workshop Proceedings, volume 4276, 2026. Published September 29, 2026.

The [workshop](https://perso.ens-lyon.fr/francois.schwarzentruber/research/events/logicnn2026/)
took place at FLoC in Lisbon, Portugal, on July 25, 2026.
