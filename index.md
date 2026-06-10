---
layout: default
title: Home
---

## CV / 制作物

- [CV](/cv/)
- [制作物](/works/)


## Recent Tech memo

{% assign sorted_techmemo = site.techmemo | sort: "date" | reverse %}

{% for post in sorted_techmemo limit:3 %}
- [{{ post.title }}]({{ post.url }})
  ({{ post.date | date: "%Y-%m-%d" }})
{% endfor %}

[More](/techmemo/)

## 雑記

{% assign sorted_posts = site.posts | sort: "date" | reverse %}

{% for post in sorted_posts limit:3 %}
- [{{ post.title }}]({{ post.url }})
  ({{ post.date | date: "%Y-%m-%d" }})
{% endfor %}

[More](/posts/)