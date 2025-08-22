---
layout: default
title: Overview
---

# Index of Pages

<ul>
{% assign pages_sorted = site.pages | sort: "name" %}
{% for p in pages_sorted %}
  {% unless p.name == "test.md" %}
    <li><a href="{{ p.url | relative_url }}">{{ p.title | default: p.name | remove: ".md" | capitalize }}</a></li>
  {% endunless %}
{% endfor %}
</ul>