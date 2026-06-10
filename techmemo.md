---
layout: default
title: Tech memo
permalink: /techmemo/
---

# Tech memo

{% assign sorted_techmemo = site.techmemo | sort: "date" | reverse %}

{% for post in sorted_techmemo %}
- [{{ post.title }}]({{ post.url }})
  ({{ post.date | date: "%Y-%m-%d" }})
{% endfor %}
