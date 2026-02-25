---
layout: page
title: 分类
permalink: /categories/
---

<ul>
  {% for category in site.categories %}
  <li>
    <strong>{{ category[0] }}</strong> ({{ category[1].size }})
    <ul>
      {% for post in category[1] %}
      <li><a href="{{ post.url | relative_url }}">{{ post.title }}</a></li>
      {% endfor %}
    </ul>
  </li>
  {% endfor %}
</ul>

