---
layout: page
title: Willkommen
permalink: /
---

Homepage von DL0MUC - Der Clubstation sowie von DB0MUC - Der automatischen Station des Chaos Computer Club München

{% include image.html url="/assets/pages/qsl_01.jpg" width=600 align="center" %}


| Neben den Grundsätzen der offenen und freien Kommunikation, setzen wir uns stark für OpenSource Soft- und Hardware ein. <br> <br> Denn dies ist die Basis um den Selbstbau von Funktechnik und die Entwicklung neuer Betriebsarten im Amateurfunk zu ermöglichen und zu erhalten. 
| - 
|   

<br style="clear: both;"> 
**Aktivitätsabend:** Aktuell findet leider kein regelmäßiger Termin statt.

### Letzte Blogeinträge

Ältere Einträge finden sich unter <a href="/bloglisting" title="Blog">Blog</a>

<div class="post">
{% for post in site.posts %}
{% if forloop.index <= 6 %}
<hr>
    <div class="post-preview">
        <a href="{{ post.url | prepend: site.baseurl }}.html">
            <h3 class="post-title"> {{ post.title }} </h3>
            {% if post.subtitle %}
            <h4 class="post-subtitle"> {{ post.subtitle }} </h4>
            {% endif %}
        </a>
        {{ post.excerpt }}
        <p class="post-meta" style="margin-bottom:5px">Eintrag von {{ post.author }} am {{ post.date | date: "%-d. %B %Y" }}</p>
    </div>
{% endif %}
{% endfor %}
</div>
