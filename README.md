# 个人博客写作指南

本博客基于 [Hexo](https://hexo.io/) 搭建，托管于 GitHub Pages。

- **线上地址**: [https://sza0415.github.io/](https://sza0415.github.io/)
- **本地后台**: [http://localhost:4000/admin/](http://localhost:4000/admin/)

---

## 🚀 快速开始

### 1. 启动写作服务
每次写博客前，打开终端进入项目目录，运行：
```bash
npx hexo server
```
服务启动后，保持终端窗口开启。

### 2. 进入写作后台
在浏览器访问：
👉 **[http://localhost:4000/admin/](http://localhost:4000/admin/)**

- **用户名**: `sza0415`
- **密码**: `szaZIANG0415!` (或你后来修改的密码)

### 3. 写作与发布
1. 点击右上角 **New Post** 创建新文章。
2. 撰写内容（支持 Markdown，可直接粘贴图片）。
3. 点击 **Publish** 发布文章（此时文章进入 `_posts` 目录，但仅本地可见）。
4. **【重要】** 在文章列表页，点击上方的 **Deploy** 按钮。
   - 等待约 30 秒，直到出现 "Deploy done" 提示。
   - 这会将文章推送到 GitHub Pages，所有人可见。

---

## 🛠 常用命令

如果你更喜欢用命令行操作：

| 操作 | 命令 | 说明 |
| :--- | :--- | :--- |
| **启动预览** | `npx hexo server` | 启动本地服务器 (localhost:4000) |
| **新建文章** | `npx hexo new "标题"` | 创建一篇新文章 |
| **一键部署** | `npx hexo clean && npx hexo deploy` | 清理缓存并发布到线上 |
| **备份源码** | `git add . && git commit -m "更新" && git push` | 备份源文件到 GitHub (建议定期执行) |

## ⚠️ 注意事项

1. **图片粘贴**: 在后台粘贴图片时，它会自动生成路径。如果手动插入，请使用 `/images/文件名.png`。
2. **草稿预览**: 本地已开启草稿预览 (`render_drafts: true`)，你可以在后台保存为 Draft 边写边看，写好后再 Publish。
3. **强制刷新**: 部署后如果线上没变化，请尝试强制刷新浏览器 (`Ctrl+F5` / `Cmd+Shift+R`)。
