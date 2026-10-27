---
layout: archive
title: "Sitemap"
permalink: /sitemap/
author_profile: true
---

{% include base_path %}

A list of the main pages and publication summaries. An [XML sitemap]({{ base_path }}/sitemap.xml) is also available.

## Pages

- [About me]({{ '/' | relative_url }})
- [Publications]({{ '/publications/' | relative_url }})

## Publications and preprints

{% assign sorted_publications = site.publications | sort: 'date' | reverse %}
<ul>
{% for post in sorted_publications %}
  <li><a href="{{ post.url | relative_url }}">{{ post.title }}</a> ({{ post.date | date: '%Y' }})</li>
{% endfor %}
</ul>
