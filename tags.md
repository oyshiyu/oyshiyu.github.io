---
layout: page
title: 标签
permalink: /tags/
---

<ul>
  {% for tag in site.tags %}
  <li>
    <strong>{{ tag[0] }}</strong> ({{ tag[1].size }})
    <ul>
      {% for post in tag[1] %}
      <li><a href="{{ post.url | relative_url }}">{{ post.title }}</a></li>
      {% endfor %}
    </ul>
  </li>
  {% endfor %}
</ul>

