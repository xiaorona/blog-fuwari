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
  @media (max-width: 640px) {
    .friend-grid {
      grid-template-columns: repeat(2, minmax(0, 1fr));
      gap: 0.75rem;
    }
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
    text-align: center;
  }
  .friend-avatar-container {
    width: 56px;
    height: 56px;
    margin-bottom: 0.5rem;
  }
  .friend-avatar {
    width: 100%;
    height: 100%;
    border-radius: 50%;
    object-fit: cover;
    max-width: 56px;
    max-height: 56px;
  }
  .friend-name {
    font-weight: 500;
    color: var(--link-color);
    margin-bottom: 0.25rem;
    font-size: 0.95rem;
    word-break: break-word;
  }
  .friend-desc {
    color: var(--text-secondary);
    font-size: 0.85rem;
    line-height: 1.4;
    word-break: break-word;
  }
---

## 🎯 友链展示

<div class="friend-grid">
  <!-- 友链卡片1 -->
  <a href="https://astro.build" target="_blank" rel="noopener" class="friend-card">
    <div class="friend-avatar-container">
      <img class="friend-avatar" src="https://astro.build/favicon.svg" alt="Astro">
    </div>
    <div class="friend-name">Astro</div>
    <div class="friend-desc">静态站点生成器</div>
  </a>

  <!-- 友链卡片2 -->
  <a href="https://github.com/saicaca/fuwari" target="_blank" rel="noopener" class="friend-card">
    <div class="friend-avatar-container">
      <img class="friend-avatar" src="https://github.githubassets.com/favicons/favicon.png" alt="Fuwari">
    </div>
    <div class="friend-name">Fuwari</div>
    <div class="friend-desc">Astro主题</div>
  </a>
</div>

## 📝 申请友链
（保持原有邮箱和格式不变）