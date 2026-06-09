---
layout: default
title: Home
---

# Diary

{% for post in site.posts %}
- [{{ post.title }}]({{ post.url }})
  ({{ post.date | date: "%Y-%m-%d" }})
{% endfor %}