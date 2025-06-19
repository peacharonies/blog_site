---
layout: default
title: Home
---

# The Peachy Observer

**Links:** [GitHub](https://github.com/jarkanni) | [Minecraft Server](https://yellowcake.peacharonies.com)

---

{% for post in site.posts %}
  <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
  <p>{{ post.date | date: "%B %d, %Y at %I:%M %p" }}</p>
  <p>{{ post.excerpt | strip_html | truncatewords: 13 }}</p>
  <hr>
{% endfor %}
