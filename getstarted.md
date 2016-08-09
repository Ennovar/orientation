---
layout: page
permalink: /getstarted/
title: get started
description: How to get up to speed and start working
---

<ul class="post-list">
{% for post in site.getstarted %}
    <li>
        <h2><a class="post-title" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a></h2>
        <p class="post-meta">{{ post.date | date: '%B %-d, %Y — %H:%M' }}</p>
      </li>
{% endfor %}
</ul>
