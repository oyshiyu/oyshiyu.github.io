---
layout: home
title: 首页
list_title: 最新文章
---

<div class="hero-panel">
  <section>
    <p class="hero-kicker">oyshiyu.github.io</p>
    <h1 class="hero-title">记录研究、工程与写作过程</h1>
    <p class="hero-lead">这是一个中文个人博客。</p>
    <div class="hero-actions">
      <a class="btn-pill" href="{{ '/blog/' | relative_url }}">进入博客</a>
      <a class="btn-pill btn-pill--ghost" href="{{ '/about/' | relative_url }}">关于本站</a>
    </div>
  </section>

  <aside class="hero-note">
    <h2>写作方向</h2>
    <ul class="hero-list">
      <li>技术实践与工具链</li>
      <li>研究笔记与论文整理</li>
      <li>项目记录与过程复盘</li>
    </ul>
    <p class="hero-mini">分类和标签。</p>
    <div class="chip-row">
      <span class="meta-chip">技术实践</span>
      <span class="meta-chip">研究笔记</span>
      <span class="meta-chip">项目记录</span>
      <span class="meta-chip">阅读笔记</span>
      <span class="meta-chip">随想</span>
    </div>
  </aside>
</div>

<div class="quick-grid">
  <a class="quick-card" href="{{ '/blog/' | relative_url }}">
    <span class="quick-card__label">Archive</span>
    <strong>博客归档</strong>
    <p>按年份浏览文章，并查看当前分类与标签统计。</p>
  </a>
  <a class="quick-card" href="{{ '/categories/' | relative_url }}">
    <span class="quick-card__label">Categories</span>
    <strong>分类索引</strong>
    <p>按内容大类浏览，适合查找主题相关的文章。</p>
  </a>
  <a class="quick-card" href="{{ '/tags/' | relative_url }}">
    <span class="quick-card__label">Tags</span>
    <strong>标签索引</strong>
    <p>按技术栈、方法和工具标签进行快速定位。</p>
  </a>
</div>
