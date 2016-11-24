---
layout: page
title: Willkommen
permalink: /
---

Homepage von DL0MUC - Der Clubstation des Chaos Computer Clubs München 
sowie von DB0MUC - Der automatischen Station des Chaos Computer Club München

## Neuigkeiten

Ältere Neuigkeite finden sich unter <a href="/news" title="News">News</a>

<ul id="posts" class="posts">
{% for post in site.posts %}
    <li>
        <span class="post-date">{{ post.date | date: "%b %-d, %Y" }}</span>
        <a class="post-link" href="{{ post.url | prepend: site.baseurl }}.html">{{ post.title }}</a>
    </li>
{% endfor %}
</ul>
