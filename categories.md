---
layout: page
title: 分类
permalink: /categories/
---

<div class="taxonomy-shell">
  <section class="surface-card">
    <h2>分类索引</h2>
    <p>分类用于组织内容的大方向，便于浏览同一类主题下的文章。</p>
  </section>

  {% for category in site.categories %}
  <section class="surface-card taxonomy-block">
    <h2>
      {{ category[0] }}
      <em class="meta-chip__count">{{ category[1].size }}</em>
    </h2>
    <ul class="taxonomy-posts">
      {% for post in category[1] %}
      <li><a href="{{ post.url | relative_url }}">{{ post.title }}</a></li>
      {% endfor %}
    </ul>
  </section>
  {% endfor %}
</div>
