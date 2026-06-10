---
layout: default
title: Diary
permalink: /diary/
---

# Diary

{% assign sorted_diary = site.diary | sort: "date" | reverse %}

{% for post in sorted_diary %}
- [{{ post.title }}]({{ post.url }})
  ({{ post.date | date: "%Y-%m-%d" }})
{% endfor %}
