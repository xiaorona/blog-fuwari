---
# src/pages/friendlink.md
layout: ../../layouts/MainGridLayout.astro
title: 友情链接
description: 我的博客友链列表
style: |
  .friend-grid {
    display: grid;
    grid-template-columns: repeat(2, minmax(0, 1fr));
    gap: 1.25rem;
    margin: 1.5rem 0;
  }
  @media (max-width: 640px) {
    .friend-grid {
      gap: 0.8rem;
    }
  }
  .friend-card {
    display: flex;
    flex-direction: column;
    align-items: center;
    padding: 1.25rem 1rem;
    border-radius: 12px; /* 增大圆角 */
    background: var(--card-bg);
    border: 1px solid var(--border-color);
    box-shadow: 0 2px 6px rgba(0,0,0,0.05);
    transition: all 0.25s ease;
    height: 100%;
    text-align: center;
  }
  .friend-card:hover {
    transform: translateY(-2px);
    box-shadow: 0 4px 12px rgba(0,0,0,0.1);
  }
  .friend-avatar-container {
    width: 64px;
    height: 64px;
    margin-bottom: 0.75rem;
    border-radius: 12px; /* 头像容器圆角 */
    overflow: hidden;
    background: var(--bg-secondary);
    display: flex;
    align-items: center;
    justify-content: center;
  }
  .friend-avatar {
    width: 56px;
    height: 56px;
    border-radius: 8px; /* 头像图片圆角 */
    object-fit: cover;
  }
  .friend-name {
    font-weight: 600;
    color: var(--text-primary);
    margin: 0.5rem 0 0.25rem;
    font-size: 1rem;
  }
  .friend-desc {
    color: var(--text-secondary);
    font-size: 0.9rem;
    line-height: 1.5;
    opacity: 0.9;
  }
  .friend-link {
    margin-top: 0.75rem;
    font-size: 0.85rem;
    color: var(--link-color);
    display: inline-flex;
    align-items: center;
    gap: 0.25rem;
  }
---

## 🎯 友链展示

<div class="friend-grid">
  <!-- 友链卡片1 -->
  <div class="friend-card">
    <div class="friend-avatar-container">
      <img class="friend-avatar" src="https://pic.qqans.com/up/2020-12/16070652272345929.jpg" alt="Astro">
    </div>
    <h3 class="friend-name">Astro</h3>
    <p class="friend-desc">现代静态站点生成器</p>
    <a href="https://astro.build" target="_blank" rel="noopener" class="friend-link">
      访问网站 ↗
    </a>
  </div>

  <!-- 友链卡片2 -->
  <div class="friend-card">
    <div class="friend-avatar-container">
      <img class="friend-avatar" src="https://pic.qqans.com/up/2020-12/16070652276806379.jpg" alt="Fuwari">
    </div>
    <h3 class="friend-name">Fuwari</h3>
    <p class="friend-desc">轻量级Astro主题</p>
    <a href="https://github.com/saicaca/fuwari" target="_blank" rel="noopener" class="friend-link">
      访问项目 ↗
    </a>
  </div>
</div>

## 📝 申请友链
（保持原有邮箱和格式不变）