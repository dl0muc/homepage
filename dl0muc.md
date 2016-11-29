---
layout: page
title: DL0MUC
description: Clubstation DL0MUC
permalink: /dl0muc/
categories: none
---

Unsere Clubstation DL0MUC befindet sich in den Räumen des Chaos Computer Club München. 

{% include image.html url="/assets/pages/shack_01.jpg" caption="Shack im Studio" width=600 align="center" %}
<br style="clear: both;"> 

Die Station ist aktuell ausgestattet mit einem ICOM IC-9100 KW/VHF/UHF Transceiver (100W), einer 600W PA sowie einem Shack-Rechner mit der geläufigsten OpenSource HAM-Software.

Im selben Raum befindet sich auch das [HF-Labor](/hf-labor/) des µC³.

Die Ausstattung wird permanent erweitert und 

Für weitere Details siehe auch: 

<ul class="listing">
{% for page in site.pages %}
  {% if page.categories contains 'dl0muc' %}
  <li class="listing-item">
    <a href="{{ page.url }}.html" title="{{ page.title }}">{{ page.title }}</a>
  </li>
  {% endif %}
{% endfor %}
</ul>