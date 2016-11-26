---
layout: page
title: Willkommen
permalink: /
---

Homepage von DL0MUC - Der Clubstation des Chaos Computer Clubs München 
sowie von DB0MUC - Der automatischen Station des Chaos Computer Club München

### Letzte Blogeinträge

Ältere Einträge finden sich unter <a href="/bloglisting" title="Blog">Blog</a>

<div class="post">
{% for post in site.posts %}
{% if forloop.index <= 6 %}
    <div class="post-preview">
        <a href="{{ post.url | prepend: site.baseurl }}.html">
            <h3 class="post-title"> {{ post.title }} </h3>
            {% if post.subtitle %}
            <h4 class="post-subtitle"> {{ post.subtitle }} </h4>
            {% endif %}
        </a>
        <p class="post-meta" style="margin-bottom:5px">Eintrag von {{ post.author }} am {{ post.date | date: "%-d. %B %Y" }}</p>
    </div>
{% endif %}
{% endfor %}
</div>
