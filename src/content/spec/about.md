---
# src/pages/friendlink.md
layout: ../../layouts/MainGridLayout.astro
title: 友情链接
description: 我的博客友链列表
style: |
  .friend-grid {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(240px, 1fr));
    gap: 1.5rem;
    margin: 1.5rem 0;
  }
  .friend-card {
    display: flex;
    flex-direction: column;
    align-items: center;
    padding: 1rem;
    border-radius: 8px;
    background: var(--card-bg);
    border: 1px solid var(--border-color);
    transition: transform 0.2s;
    height: 100%;
  }
  .friend-card:hover {
    transform: translateY(-3px);
  }
  .friend-avatar {
    width: 64px;
    height: 64px;
    border-radius: 50%;
    object-fit: cover;
    margin-bottom: 0.75rem;
  }
  .friend-name {
    font-weight: 500;
    color: var(--link-color);
    text-align: center;
    margin-bottom: 0.25rem;
  }
  .friend-desc {
    color: var(--text-secondary);
    text-align: center;
    font-size: 0.9rem;
    line-height: 1.4;
  }
---

## 🎯 友链展示

<div class="friend-grid">
  <!-- 友链卡片1 -->
  <a href="https://astro.build" target="_blank" rel="noopener" class="friend-card">
    <img class="friend-avatar" src="https://astro.build/favicon.svg" alt="Astro">
    <div class="friend-name">Astro 官方</div>
    <div class="friend-desc">现代静态站点生成器</div>
  </a>

  <!-- 友链卡片2 -->
  <a href="https://github.com/saicaca/fuwari" target="_blank" rel="noopener" class="friend-card">
    <img class="friend-avatar" src="https://github.githubassets.com/favicons/favicon.png" alt="Fuwari">
    <div class="friend-name">Fuwari主题</div>
    <div class="friend-desc">轻量级Astro博客主题</div>
  </a>
</div>

## 📝 申请友链
请按格式发送邮件至：

📮 [contact@example.com](mailto:contact@example.com?subject=友链申请&body=名称：您的网站名%0A链接：https://example.com%0A描述：一句话介绍%0A头像：图片URL（可选）)

申请格式：
```plaintext
名称：您的网站名
链接：https://example.com
描述：一句话介绍
头像：图片URL（可选）