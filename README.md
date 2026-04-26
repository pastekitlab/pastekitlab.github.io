# 我的 Hugo 博客

基于 Hugo 构建的静态博客网站，使用 GitHub Actions 自动部署到 GitHub Pages。

## 本地开发

### 安装 Hugo

```bash
# macOS
brew install hugo

# 或从官网下载
# https://gohugo.io/installation/
```

### 运行本地服务器

```bash
hugo server -D
```

访问 http://localhost:1313 查看网站。

### 创建新文章

```bash
hugo new posts/my-new-post.md
```

### 构建网站

```bash
hugo --minify
```

生成的静态文件位于 `public/` 目录。

## 部署到子域名

### 1. 配置 DNS

在你的域名服务商处添加 CNAME 记录：
- 主机记录：`blog`（或其他子域名）
- 记录值：`yourusername.github.io`

### 2. 更新 baseURL

在 `hugo.toml` 中修改：
```toml
baseURL = 'https://blog.yourdomain.com/'
```

### 3. 创建 CNAME 文件（可选）

如果使用自定义域名而非 GitHub 提供的子域名，在 `static/` 目录创建 `CNAME` 文件：
```
blog.yourdomain.com
```

### 4. 推送并部署

```bash
git add .
git commit -m "迁移到 Hugo 博客框架"
git push origin main
```

GitHub Actions 会自动构建并部署。

## 主题

使用 [Ananke](https://github.com/theNewDynamic/gohugo-theme-ananke) 主题。
