---
layout: default
title: Overview
nav_order: 3
---

# Overview

This page provides an overview of the available sections of the site.  
Here you’ll find quick links to the main topics, organized in navigation order,  
so you can easily explore the content step by step.

<ul>
{% assign pages_sorted = site.pages | sort: "nav_order" %}
{% for p in pages_sorted %}
  {% if p.name contains ".md" and p.name != "Overview.md" %}
    <li><a href="{{ p.url | relative_url }}">{{ p.title | default: p.name | remove: ".md" | capitalize }}</a></li>
    {% if forloop.index == 2 %}
      <hr>
    {% endif %}
  {% endif %}
{% endfor %}
</ul>
