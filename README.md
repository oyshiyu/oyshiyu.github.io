# oyshiyu.github.io（Jekyll 博客骨架）

这是一个用于 GitHub Pages 的 Jekyll 中文博客最小骨架版本。

## 当前配置（v1）

- 站点类型：仅博客
- 语言：中文
- 技术栈：Jekyll
- 评论 / 搜索 / 统计：暂未启用
- 自定义域名：暂未配置

## 本地预览（可选）

前提：本机已安装 Ruby、Bundler。

```bash
bundle install
bundle exec jekyll serve
```

默认访问地址：

- `http://127.0.0.1:4000/`

## 发布到 GitHub Pages（用户站点）

1. 在 GitHub 创建仓库：`oyshiyu.github.io`
2. 将当前目录内容推送到该仓库默认分支（通常是 `main`）
3. 在仓库设置中打开 Pages（若未自动启用）
4. 选择 `Deploy from a branch`，分支选 `main`，目录选 `/ (root)`
5. 等待构建完成后访问：
   - `https://oyshiyu.github.io`

## 文章 Front Matter（当前约定）

```yaml
---
layout: post
title: "文章标题"
date: 2026-02-25 20:00:00 +0800
categories: [研究笔记]
tags: [电力系统, 优化]
description: "一句话摘要"
---
```

## 建议的分类与标签（v1）

分类：

- 技术实践
- 研究笔记
- 项目记录
- 阅读笔记
- 随想

标签种子（可逐步扩展）：

- python
- github
- github-pages
- jekyll
- latex
- 论文
- 科研
- 电力系统
- 优化
- 仿真
- 数据分析
- 可视化
- 工具链
- 效率
- 笔记

