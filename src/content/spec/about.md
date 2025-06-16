---
# src/pages/about.md
layout: "@layouts/MainLayout.astro"
title: "关于"
avatar: "/images/demo-avatar.png"
social:
  github: "https://github.com/yourname"
  twitter: "https://twitter.com/yourname"
---

<div class="text-center mb-8">
  <img 
    src="{frontmatter.avatar}" 
    alt="头像" 
    class="w-32 h-32 rounded-full mx-auto shadow-lg border-4 border-white dark:border-gray-800"
  >
  <h1 class="text-3xl font-bold mt-4">你的名字</h1>
  <p class="text-gray-600 dark:text-gray-400">开发者 | 技术写作者</p>
</div>

<div class="prose dark:prose-invert max-w-2xl mx-auto">
  
  ## 👋 简介
  
  你好！我是**{frontmatter.title.split(' ')[0]}**，目前专注于：
  
  - 🌐 Web 开发与开源项目
  - ✍️ 技术博客写作
  - 🎨 偶尔设计些小东西

  ## 🛠️ 技术栈
  
  <div class="flex flex-wrap gap-2 my-4">
    <span class="px-3 py-1 bg-blue-100 dark:bg-blue-900 rounded-full text-sm">JavaScript</span>
    <span class="px-3 py-1 bg-purple-100 dark:bg-purple-900 rounded-full text-sm">Astro</span>
    <span class="px-3 py-1 bg-green-100 dark:bg-green-900 rounded-full text-sm">React</span>
  </div>

  ## 📫 联系我

  <div class="flex gap-4 justify-center mt-6">
    <a href="{frontmatter.social.github}" target="_blank" class="hover:scale-110 transition">
      <svg class="w-6 h-6" fill="currentColor" viewBox="0 0 24 24"><path d="M12..."/></svg>
    </a>
    <a href="{frontmatter.social.twitter}" target="_blank" class="hover:scale-110 transition">
      <svg class="w-6 h-6" fill="currentColor" viewBox="0 0 24 24"><path d="M23..."/></svg>
    </a>
  </div>
</div>