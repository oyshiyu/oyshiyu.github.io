---
layout: page
title: 标签
permalink: /tags/
---

<div class="taxonomy-shell">
  <section class="surface-card">
    <h2>标签索引</h2>
    <p>标签用于记录技术栈、方法或工具名称，粒度比分类更细。</p>
  </section>

  {% for tag in site.tags %}
  <section class="surface-card taxonomy-block">
    <h2>
      #{{ tag[0] }}
      <em class="meta-chip__count">{{ tag[1].size }}</em>
    </h2>
    <ul class="taxonomy-posts">
      {% for post in tag[1] %}
      <li><a href="{{ post.url | relative_url }}">{{ post.title }}</a></li>
      {% endfor %}
    </ul>
  </section>
  {% endfor %}
</div>
