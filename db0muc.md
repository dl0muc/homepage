---
layout: page
title: DB0MUC
description: Automatische Station DB0MUC
permalink: /db0muc/
categories: none
---

Seit dem 01.11.2016 haben wir das Rufzeichen *DB0MUC* für den Betrieb einer automatischen Station erhalten. Folgende Frequenzen und Betriebsarten wurden uns zugeteilt:

| Typ       | Frequenz    | Duplexabstand | Bandbreite | Einsatzzweck              | max. Leistung | In Betrieb |
| --------- | ----------- | ------------- | ---------- | ------------------------- | ------------- | ---------- |
| APRS      | 144.800 MHz | -             | 12.0 kHz   | APRS-Digi                 | 15.0 W        | Ja         |
| Digi      | 438.450 MHz | -7.6 MHz      | 25.0 kHz   | Full-Duplex Digipeater    | 15.0 W        | Nein       |
| Digi (NB) | 439.450 MHz | -7.6 MHz      | 12.5 kHz   | Digitale Sprache          | 15.0 W        | Nein       |

### Unterseiten

<ul class="listing">
{% for page in site.pages %}
  {% if page.categories contains 'db0muc' %}
  <li class="listing-item">
    <a href="{{ page.url }}" title="{{ page.title }}">{{ page.title }}</a>
  </li>
  {% endif %}
{% endfor %}
</ul>
