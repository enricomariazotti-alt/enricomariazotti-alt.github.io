---
layout: default
title: Test
---

# Index of Markdown Files

<ul>
{% assign pages_sorted = site.pages | sort: "path" %}
{% for p in pages_sorted %}
  {% if p.extname == ".md" and p.path != "test.md" and p.url %}
    <li><a href="{{ p.url | relative_url }}">{{ p.title | default: p.path }}</a></li>
  {% endif %}
{% endfor %}
</ul>