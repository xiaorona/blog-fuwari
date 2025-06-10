---
# src/pages/friendlink.md
layout: ../../layouts/MainGridLayout.astro
title: 友情链接
description: 我的博客友链列表
style: |
  .friend-table {
    width: 100%;
    border-collapse: collapse;
    margin: 1.5rem 0;
  }
  .friend-table tr {
    border-bottom: 1px solid var(--border-color);
  }
  .friend-table td {
    padding: 1rem;
    vertical-align: middle;
    height: 72px; /* 固定行高确保垂直居中 */
  }
  .friend-avatar {
    width: 48px;
    height: 48px;
    border-radius: 50%;
    object-fit: cover;
    display: block;
    margin: 0 auto;
  }
  .friend-link {
    font-weight: 500;
    color: var(--link-color);
    text-decoration: none;
  }
  .friend-desc {
    color: var(--text-secondary);
    line-height: 1.5;
  }
---

## 🎯 友链展示

<table class="friend-table">
  <tr>
    <td style="width: 80px; text-align: center;">
      <img class="friend-avatar" src="https://astro.build/favicon.svg" alt="Astro" width="48" height="48">
    </td>
    <td>
      <a class="friend-link" href="https://astro.build" target="_blank" rel="noopener">Astro 官方</a>
      <p class="friend-desc">现代静态站点生成器，适合内容驱动型网站开发</p>
    </td>
  </tr>
  <tr>
    <td style="width: 80px; text-align: center;">
      <img class="friend-avatar" src="https://github.githubassets.com/favicons/favicon.png" alt="GitHub" width="48" height="48">
    </td>
    <td>
      <a class="friend-link" href="https://github.com/saicaca/fuwari" target="_blank" rel="noopener">Fuwari主题</a>
      <p class="friend-desc">轻量级Astro博客主题，简洁高效的设计风格</p>
    </td>
  </tr>
</table>

## 📝 申请友链
请按以下格式发送邮件至：

📮 [contact@example.com](mailto:contact@example.com?subject=友链申请&body=名称：您的网站名%0A链接：https://example.com%0A描述：一句话介绍（20字内）%0A头像：图片URL（可选）)

申请格式：
```plaintext
名称：您的网站名
链接：https://example.com
描述：一句话介绍（20字内）
头像：图片URL（可选）