---
layout: page
title: Projekte
permalink: /projects/
---

Hier findet sich eine Liste von Projekten welche im Rahmen der DL0MUC Clubstation enstanden sind.

<ul class="listing">
{% for page in site.pages %}
  {% if page.categories contains 'project' %}
  <li class="listing-item">
    <a href="{{ page.url }}" title="{{ page.title }}">{{ page.title }}</a>
  </li>
  {% endif %}
{% endfor %}
</ul>
