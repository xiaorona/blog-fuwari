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
  .friend-table td {
    padding: 12px 16px;
    vertical-align: middle;
    border-bottom: 1px solid var(--border-color);
  }
  .friend-avatar {
    width: 40px;
    height: 40px;
    border-radius: 50%;
    object-fit: cover;
  }
---

## 🎯 友链展示

<table class="friend-table">
  <tr>
    <td><img class="friend-avatar" src="https://astro.build/favicon.svg" alt="Astro"></td>
    <td><a href="https://astro.build" target="_blank" rel="noopener">Astro 官方</a></td>
    <td>现代静态站点生成器</td>
  </tr>
  <tr>
    <td><img class="friend-avatar" src="https://github.githubassets.com/favicons/favicon.png" alt="GitHub"></td>
    <td><a href="https://github.com/saicaca/fuwari" target="_blank" rel="noopener">Fuwari主题</a></td>
    <td>轻量博客主题</td>
  </tr>
</table>

## 📝 申请友链
请按格式发送申请至：

📮 [contact@example.com](mailto:contact@example.com?subject=友链申请&body=名称：您的网站名%0A链接：https://example.com%0A描述：一句话介绍%0A头像：图片URL（可选）)

申请格式：
```plaintext
名称：您的网站名
链接：https://example.com
描述：一句话介绍
头像：图片URL（可选）