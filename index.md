---
layout: default
title: Home
---

{% for post in site.posts %}
  <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
  <p>{{ post.date | date: "%B %d, %Y at %I:%M %p" }}</p>
  <p>{{ post.excerpt | strip_html | truncatewords: 13 }}</p>
  <hr>
  <br>
{% endfor %}
