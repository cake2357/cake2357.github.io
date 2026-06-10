---
layout: default
title: Home
---

## CV / 制作物

- [CV →](/cv/)
- [制作物 →](/works/)


## Recent Tech memo

{% assign sorted_techmemo = site.techmemo | sort: "date" | reverse %}

{% for post in sorted_techmemo limit:3 %}
- [{{ post.title }}]({{ post.url }})
  ({{ post.date | date: "%Y-%m-%d" }})
{% endfor %}

[More →](/techmemo/)

## Recent Diary

{% assign sorted_diary = site.diary | sort: "date" | reverse %}

{% for post in sorted_diary limit:3 %}
- [{{ post.title }}]({{ post.url }})
  ({{ post.date | date: "%Y-%m-%d" }})
{% endfor %}

[More →](/diary/)