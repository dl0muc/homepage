---
layout: page
title: Aufbaulogbuch
description: Hier finden sich alle News zum Aufbau unserer Clubstation
permalink: /aufbaulogbuch/
categories: [logbuch]
---

<ul class="listing">
{% for post in site.posts %}
  {% capture y %}{{post.date | date:"%Y"}}{% endcapture %}
  {% if post.categories contains 'logbuch' %}
  {% if year != y %}
    {% assign year = y %}
    <li class="listing-seperator">{{ y }}</li>
  {% endif %}
  <li class="listing-item">
    <time datetime="{{ post.date | date:"%Y-%m-%d" }}">{{ post.date | date:"%Y-%m-%d" }}</time>
    <a href="{{ post.url }}.html" title="{{ post.title }}">{{ post.title }}</a>
  </li>
  {% endif %} 
{% endfor %}
</ul>