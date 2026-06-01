---
title : Post History
description: "Timeline of previous posts."
toc: true
toc_label: "Post History"
toc_icon: "fa-regular fa-calendar-days"
toc_sticky: true
permalink: "/history.html"
nav_id: post-history
---

{% comment %} Post History - derived from https://github.com/cotes2020/jekyll-theme-chirpy {% endcomment %}

<div id="archives">
    {% for post in site.posts %}
    {% assign cur_year = post.date | date: '%Y' %}

    {% if cur_year != last_year %}
        {% unless forloop.first %}</ul>{% endunless %}

        <h2 id="{{ cur_year }}">{{ cur_year }}</h2>
        {{ '<ul class="list-unstyled">' }}

        {% assign last_year = cur_year %}
    {% endif %}

    <li>
        {% assign ts = post.date | date: '%s' %}
        <span class="date day">{{ post.date | date: '%d' }}</span>
        <span class="date month small text-muted ms-1">{{ post.date | date: '%b' }}</span>
        <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
    </li>

    {% if forloop.last %}</ul>{% endif %}
    {% endfor %}
</div>