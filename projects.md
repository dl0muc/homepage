---
layout: page
title: Projekte
description: Hier findet sich eine Liste von Projekten welche im Rahmen der DL0MUC Clubstation entstanden sind
permalink: /projects/
categories: none
---

<ul class="listing">
{% for page in site.pages %}
  {% if page.categories contains 'project' %}
  <li class="listing-item">
    <a href="{{ page.url }}" title="{{ page.title }}">{{ page.title }}</a>
  </li>
  {% endif %}
{% endfor %}
</ul>
