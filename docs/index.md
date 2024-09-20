---
layout: default
title: devlog
---

# devlog

<ul>
  {% for post in site.pages %}
    {% if post.path contains '.md' and post.path != 'index.md' %}
      <li><a href="/devlog{{ post.url }}">{{ post.title | escape }}</a></li>
    {% endif %}
  {% endfor %}
</ul>
