---
layout: default
title: 雑記
permalink: /posts/
---

# 雑記

{% assign sorted_posts = site.posts | sort: "date" | reverse %}

{% for post in sorted_posts %}
- [{{ post.title }}]({{ post.url }})
  ({{ post.date | date: "%Y-%m-%d" }})
{% endfor %}
