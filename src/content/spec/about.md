---
# src/pages/friendlink.md
layout: ../../layouts/MainGridLayout.astro
title: 友情链接
description: 欢迎来到我的友情链接页面
style: |
  .friend-container {
    @apply grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6 my-8;
  }
  .friend-card {
    @apply flex items-center gap-4 p-4 bg-gray-100 dark:bg-gray-800 rounded-lg hover:shadow-md transition-colors;
  }
  .friend-avatar {
    @apply w-12 h-12 rounded-full object-cover flex-shrink-0;
  }
  .friend-info h3 {
    @apply font-medium text-lg;
  }
  .friend-info p {
    @apply text-sm text-gray-600 dark:text-gray-400 mt-1;
  }
---

## 🌟 友情链接

以下是与我互换友链的伙伴们：

```astro
---
// 内联友链数据
const friendLinks = [
  {
    name: "Astro 官方文档",
    url: "https://docs.astro.build/",
    description: "Astro 框架官方文档",
    avatar: "https://astro.build/favicon.svg"
  },
  {
    name: "Fuwari GitHub",
    url: "https://github.com/saicaca/fuwari",
    description: "Fuwari 主题仓库",
    avatar: "https://github.com/saicaca.png"
  },
  {
    name: "示例友链",
    url: "https://example.com",
    description: "这是一个示例友链",
    avatar: "https://via.placeholder.com/50"
  }
];
---

<div class="friend-container">
  {
    friendLinks.map(link => (
      <a 
        href={link.url} 
        target="_blank" 
        rel="noopener noreferrer"
        class="friend-card"
      >
        <img 
          src={link.avatar} 
          alt={link.name} 
          class="friend-avatar"
          width="48"
          height="48"
        />
        <div class="friend-info">
          <h3>{link.name}</h3>
          <p>{link.description}</p>
        </div>
      </a>
    ))
  }
</div>