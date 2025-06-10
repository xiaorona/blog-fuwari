## 友链列表

<!-- 使用 Astro 组件语法嵌入友链数据 -->
<script>
  // 定义友链数据（也可以从外部 JSON 导入）
  const friendLinks = [
    {
      name: "Astro 官方文档",
      url: "https://docs.astro.build/",
      description: "Astro 的官方文档",
      avatar: "https://astro.build/favicon.svg"
    },
    {
      name: "Fuwari GitHub",
      url: "https://github.com/saicaca/fuwari",
      description: "Fuwari 主题的 GitHub 仓库",
      avatar: "https://github.com/saicaca.png"
    }
  ];
</script>

<!-- 渲染友链卡片 -->
<div class="friendlink-grid">
  {friendLinks.map(link => (
    <a href={link.url} target="_blank" rel="noopener noreferrer" class="friendlink-card">
      <img src={link.avatar} alt={link.name} class="avatar" />
      <div class="info">
        <h3>{link.name}</h3>
        <p>{link.description}</p>
      </div>
    </a>
  ))}
</div>

<style>
  .friendlink-grid {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
    gap: 1.5rem;
    margin: 2rem 0;
  }
  .friendlink-card {
    display: flex;
    align-items: center;
    gap: 1rem;
    padding: 1rem;
    border-radius: 8px;
    background: var(--ec-color-bg-secondary);
    transition: transform 0.2s ease;
  }
  .friendlink-card:hover {
    transform: translateY(-4px);
  }
  .avatar {
    width: 50px;
    height: 50px;
    border-radius: 50%;
    object-fit: cover;
  }
</style>