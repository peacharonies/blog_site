---
layout: default
title: Home
---

{% for post in site.posts %}
    <h1><a href="{{ post.url }}">{{ post.title }}</a></h1>
    <p>{{ post.date | date: "%B %d, %Y at %I:%M %p" }}</p>
    <p>{{ post.content | strip_html | truncatewords: 13 }}</p>
{% endfor %}
