---
layout: default
title: Home
---

# Diary

{% for post in site.diary %}
- [{{ post.title }}]({{ post.url }})
  ({{ post.date | date: "%Y-%m-%d" }})
{% endfor %}