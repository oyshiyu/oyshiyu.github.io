---
layout: page
title: 博客
permalink: /blog/
---

{% assign posts_by_year = site.posts | group_by_exp: "post", "post.date | date: '%Y'" %}

<div class="archive-shell">
  <section class="surface-card archive-summary">
    <div>
      <h2>博客归档</h2>
      <p>按年份查看文章，同时保留一份简洁的分类与标签概览，便于后续扩展主题页。</p>
    </div>
    <div class="stat-grid">
      <div class="stat-card">
        <p class="stat-card__label">文章</p>
        <p class="stat-card__value">{{ site.posts | size }}</p>
      </div>
      <div class="stat-card">
        <p class="stat-card__label">分类</p>
        <p class="stat-card__value">{{ site.categories | size }}</p>
      </div>
      <div class="stat-card">
        <p class="stat-card__label">标签</p>
        <p class="stat-card__value">{{ site.tags | size }}</p>
      </div>
    </div>
  </section>

  <section class="surface-card">
    <h2>全部文章</h2>
    {% for year in posts_by_year %}
    <div class="archive-year">
      <h3>{{ year.name }}</h3>
      <ul class="post-link-list">
        {% for post in year.items %}
        <li>
          <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
          <time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%Y-%m-%d" }}</time>
        </li>
        {% endfor %}
      </ul>
    </div>
    {% endfor %}
  </section>

  <section class="surface-card">
    <h2>分类概览</h2>
    <div class="cloud-wrap">
      {% for category in site.categories %}
      <span class="meta-chip meta-chip--accent">
        {{ category[0] }}
        <em class="meta-chip__count">{{ category[1].size }}</em>
      </span>
      {% endfor %}
    </div>
  </section>

  <section class="surface-card">
    <h2>标签概览</h2>
    <div class="cloud-wrap">
      {% for tag in site.tags %}
      <span class="meta-chip meta-chip--warm">
        #{{ tag[0] }}
        <em class="meta-chip__count">{{ tag[1].size }}</em>
      </span>
      {% endfor %}
    </div>
  </section>
</div>
