---
outline: deep
---

# 运行时 API 示例  

本页面展示了 VitePress 提供的一些**运行时 API**的使用方法。  

主要的 `useData()` API 可用于访问**当前页面**的**站点数据**、**主题数据**和**页面数据**。它既可以在 `.md` 文件中使用，也可以在 `.vue` 组件中使用：  

```md
<script setup>
import { useData } from 'vitepress'

const { theme, page, frontmatter } = useData()
</script>

## Results

### Theme Data
<pre>{{ theme }}</pre>

### Page Data
<pre>{{ page }}</pre>

### Page Frontmatter
<pre>{{ frontmatter }}</pre>
```

<script setup>
import { useData } from 'vitepress'

const { site, theme, page, frontmatter } = useData()
</script>

## Results

### Theme Data
<pre>{{ theme }}</pre>

### Page Data
<pre>{{ page }}</pre>

### Page Frontmatter
<pre>{{ frontmatter }}</pre>

## More

Check out the documentation for the [full list of runtime APIs](https://vitepress.dev/reference/runtime-api#usedata).
