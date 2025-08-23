---
layout: default
title: Overview
nav_order: 3
---

# Index of Pages

<ul>
{% assign pages_sorted = site.pages | sort: "name" %}
{% for p in pages_sorted %}
  {% if p.name contains ".md" and p.name != "test.md" %}
    <li><a href="{{ p.url | relative_url }}">{{ p.title | default: p.name | remove: ".md" | capitalize }}</a></li>
  {% endif %}
{% endfor %}
</ul>