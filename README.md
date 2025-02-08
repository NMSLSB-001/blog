# 🚀 VitePress 项目

> 基于 [VitePress](https://vitepress.dev/) 构建的静态文档站点

## 📌 功能特点
- 🚀 **超快文档加载**：基于 Vite 进行优化
- 📄 **Markdown 支持**：支持 Vue 组件 & 自定义组件
- 🌍 **多语言支持**（可选）
- 🎨 **可自定义主题**
- 🔥 **支持 Cloudflare Pages 部署**

---

## 📦 安装

### **1️⃣ 克隆项目**
```sh
git clone https://github.com/your-username/your-repo.git
cd your-repo
2️⃣ 安装依赖
sh
复制
编辑
npm install
🔧 本地开发
启动本地开发环境
sh
复制
编辑
npm run docs:dev
启动后，打开 http://localhost:5173/ 进行访问。

📦 生成静态文件
构建项目
sh
复制
编辑
npm run docs:build
构建完成后，静态文件将生成在 docs/.vitepress/dist 目录。

🚀 部署到 Cloudflare Pages（推荐）
1️⃣ 创建 Cloudflare Pages 项目
进入 Cloudflare Pages
选择 GitHub/GitLab 仓库
绑定你的 VitePress 仓库
2️⃣ 配置 Cloudflare Pages
配置项	值
框架预设	None
构建命令	npm run docs:build
发布目录	docs/.vitepress/dist
3️⃣ 绑定自定义域名（可选）
在 Cloudflare Pages 控制台 添加 自定义域
配置 Cloudflare DNS，添加 CNAME 记录
⚙️ 多语言支持（可选）
如果需要支持多语言（如 中文 & 英文），修改 docs/.vitepress/config.ts：

ts
复制
编辑
export default defineConfig({
  locales: {
    root: { label: 'English', lang: 'en', link: '/en/' },
    zh: { label: '简体中文', lang: 'zh-CN', link: '/zh/' }
  }
})
然后，在 docs/en/ 和 docs/zh/ 目录分别存放不同语言的文档。

🎨 自定义主题
VitePress 支持修改 主题样式：

scss
复制
编辑
// docs/.vitepress/theme/custom.css
:root {
  --vp-c-brand: #42b983;
  --vp-c-brand-light: #73d897;
}
并在 config.ts 里引入：

ts
复制
编辑
import './theme/custom.css'
🔥 贡献指南
欢迎提交 PR 或 Issue，改进本项目！

sh
复制
编辑
git checkout -b feature-xxx
git commit -m "✨ 添加新功能"
git push origin feature-xxx
📜 许可证
本项目采用 MIT License，自由修改和分发。

🚀 Enjoy VitePress!
