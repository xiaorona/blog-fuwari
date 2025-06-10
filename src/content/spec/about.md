---
# src/pages/friendlink.md
layout: ../../layouts/MainGridLayout.astro
title: 友情链接
description: 我的博客友链列表
style: |
  .friend-table {
    width: 100%;
    border-collapse: collapse;
    margin: 1rem 0;
  }
  .friend-table tr {
    border-bottom: 1px solid var(--border-color);
  }
  .friend-table td {
    padding: 0.75rem 1rem; /* 减少上下padding */
    vertical-align: middle;
    height: 30px; /* 降低行高 */
  }
  .friend-avatar {
    width: 30px; /* 缩小头像尺寸 */
    height: 30px;
    border-radius: 50%;
    object-fit: cover;
    display: block;
    margin: 0 auto;
  }
  .friend-link {
    font-weight: 500;
    color: var(--link-color);
    text-decoration: none;
    font-size: 0.95rem; /* 微调字号 */
  }
  .friend-desc {
    color: var(--text-secondary);
    line-height: 1.4; /* 紧凑行高 */
    font-size: 0.85rem;
    margin-top: 0.25rem;
  }
---

## 🎯 友链展示

<table class="friend-table">
  <tr>
    <td style="width: 70px; text-align: center;">
      <img class="friend-avatar" src="https://astro.build/favicon.svg" alt="Astro">
    </td>
    <td>
      <a class="friend-link" href="https://astro.build" target="_blank" rel="noopener">Astro 官方</a>
      <p class="friend-desc">现代静态站点生成器</p>
    </td>
  </tr>
  <tr>
    <td style="width: 70px; text-align: center;">
      <img class="friend-avatar" src="https://github.githubassets.com/favicons/favicon.png" alt="GitHub">
    </td>
    <td>
      <a class="friend-link" href="https://github.com/saicaca/fuwari" target="_blank" rel="noopener">Fuwari主题</a>
      <p class="friend-desc">轻量级Astro博客主题</p>
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