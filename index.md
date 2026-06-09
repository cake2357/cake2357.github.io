---
layout: home
title: Home
---

# Diary

<ul>
{% for entry in site.diary %}
  <li>
    <a href="{{ entry.url }}">
      {{ entry.title }}
    </a>
  </li>
{% endfor %}
</ul>