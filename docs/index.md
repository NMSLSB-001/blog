---
title: Redirecting...
layout: home
---

<script setup>
import { useRouter } from 'vitepress'

const router = useRouter()

// 页面加载后跳转到默认语言（如 /zh/）
router.go('/zh/')
</script>

如果未自动跳转，请 [点击这里](/zh/) 进入中文页面。
