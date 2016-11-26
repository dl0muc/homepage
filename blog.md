---
layout: page
title: Blog
description: Hier finden sich alle Neuigkeiten zu DL0MUC, DB0MUC und unseren Projekten
permalink: /bloglisting/
---

<ul class="listing">
{% for post in site.posts %}
  {% capture y %}{{post.date | date:"%Y"}}{% endcapture %}
  {% if year != y %}
    {% assign year = y %}
    <li class="listing-seperator">{{ y }}</li>
  {% endif %}
  <li class="listing-item">
    <time datetime="{{ post.date | date:"%Y-%m-%d" }}">{{ post.date | date:"%Y-%m-%d" }}</time>
    <a href="{{ post.url }}.html" title="{{ post.title }}">{{ post.title }}</a>
  </li>
{% endfor %}
</ul>
