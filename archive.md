---
layout: page
title: 博客
permalink: /blog/
---

## 全部文章

{% assign posts_by_year = site.posts | group_by_exp: "post", "post.date | date: '%Y'" %}
{% for year in posts_by_year %}
### {{ year.name }}

<ul>
  {% for post in year.items %}
  <li>
    <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
    <small>{{ post.date | date: "%Y-%m-%d" }}</small>
  </li>
  {% endfor %}
</ul>
{% endfor %}

## 分类

<ul>
  {% for category in site.categories %}
  <li>{{ category[0] }} ({{ category[1].size }})</li>
  {% endfor %}
</ul>

## 标签

<ul>
  {% for tag in site.tags %}
  <li>{{ tag[0] }} ({{ tag[1].size }})</li>
  {% endfor %}
</ul>

