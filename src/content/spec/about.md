---
# src/pages/friendlink.md
layout: ../../layouts/MainGridLayout.astro
title: 友情链接
description: 我的博客友链列表
style: |
  .friend-grid {
    display: grid;
    grid-template-columns: repeat(2, minmax(0, 1fr));
    gap: 1rem;
    margin: 1.5rem 0;
  }
  .friend-card {
    display: flex;
    flex-direction: row;
    align-items: center;
    padding: 0.8rem;
    border-radius: 12px;
    background: var(--card-bg);
    border: 1px solid var(--border-color);
    transition: transform 0.2s;
    height: 100%;
  }
  .friend-avatar {
    width: 36px;
    height: 36px;
    border-radius: 8px;
    object-fit: cover;
    margin-right: 0.8rem;
    flex-shrink: 0;
  }
  .friend-content {
    flex: 1;
    min-width: 0;
  }
  .friend-name {
    font-weight: 500;
    color: var(--text-primary);
    margin-bottom: 0.2rem;
    font-size: 0.95rem;
    white-space: nowrap;
    overflow: hidden;
    text-overflow: ellipsis;
  }
  .friend-desc {
    color: var(--text-secondary);
    font-size: 0.85rem;
    line-height: 1.4;
    display: -webkit-box;
    -webkit-line-clamp: 2;
    -webkit-box-orient: vertical;
    overflow: hidden;
  }
  @media (max-width: 640px) {
    .friend-grid {
      gap: 0.8rem;
    }
    .friend-card {
      padding: 0.7rem;
    }
    .friend-avatar {
      width: 32px;
      height: 32px;
      margin-right: 0.7rem;
    }
  }
---

## 🎯 友链展示

<div class="friend-grid">
  <!-- 友链卡片1 -->
  <a href="https://astro.build" target="_blank" rel="noopener" class="friend-card">
    <img class="friend-avatar" src="https://astro.build/favicon.svg" alt="Astro">
    <div class="friend-content">
      <div class="friend-name">Astro 官方</div>
      <div class="friend-desc">现代静态站点生成器</div>
    </div>
  </a>

  <!-- 友链卡片2 -->
  <a href="https://github.com/saicaca/fuwari" target="_blank" rel="noopener" class="friend-card">
    <img class="friend-avatar" src="https://github.githubassets.com/favicons/favicon.png" alt="Fuwari">
    <div class="friend-content">
      <div class="friend-name">Fuwari主题</div>
      <div class="friend-desc">轻量级Astro博客主题</div>
    </div>
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