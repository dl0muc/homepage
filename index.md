---
layout: page
title: Willkommen
permalink: /
---

Homepage von DL0MUC - Der Clubstation des Chaos Computer Clubs München 
sowie von DB0MUC - Der automatischen Station des Chaos Computer Club München

## Neuigkeiten

Ältere Neuigkeite finden sich unter <a href="/news" title="News">News</a>

<div class="post">
{% for post in site.posts %}
{% if forloop.index <= 2 %}
    <div class="post-preview">
        <a href="{{ post.url | prepend: site.baseurl }}">
            <h3 class="post-title"> {{ post.title }} </h3>
            {% if post.subtitle %}
            <h4 class="post-subtitle"> {{ post.subtitle }} </h4>
            {% endif %}
        </a>
        <p class="post-meta" style="margin-bottom:5px">Eintrag von {{ post.author }} on {{ post.date | date: "%B %-d, %Y" }}</p>
    </div>
{% endif %}
{% endfor %}
</div>
