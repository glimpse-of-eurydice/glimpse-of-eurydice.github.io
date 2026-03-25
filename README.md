# Josie Qiu's Blog

个人技术博客，关注AI安全、陪伴类AI评测与数字语言学。

## 部署步骤

### 1. 创建GitHub仓库

在GitHub上创建一个新仓库，命名为 `glimpse-of-eurydice.github.io`。

### 2. 推送文件

```bash
cd blog
git init
git add .
git commit -m "Initial blog setup"
git branch -M main
git remote add origin https://github.com/glimpse-of-eurydice/glimpse-of-eurydice.github.io.git
git push -u origin main
```

### 3. 启用GitHub Pages

- 进入仓库 Settings → Pages
- Source 选择 `Deploy from a branch`
- Branch 选择 `main`，文件夹选 `/ (root)`
- 点击 Save

等待1-2分钟，访问 `https://glimpse-of-eurydice.github.io` 即可看到博客。

## 发布新文章

在 `_posts/` 目录下创建新文件，命名格式：`YYYY-MM-DD-文章名.md`

文件开头加上 front matter：

```yaml
---
layout: post
title: "文章标题"
date: 2026-03-25
tags: [标签1, 标签2]
lang: zh
excerpt_text: "首页显示的摘要文字"
---
```

然后直接写Markdown正文即可。

## 本地预览（可选）

```bash
gem install bundler jekyll
bundle install
bundle exec jekyll serve
```

然后访问 `http://localhost:4000`。
