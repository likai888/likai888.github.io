---
layout: post
title: "GitHub 基础知识"
date: 2025-04-01
---

今天受到启发，准备开始写blog。第一步是找到一个合适的平台，发现github很不错，于是就有了从学习github开始的第一篇blog文章。
这篇文章记录一些很基础的知识，是等以后需要更多知识的时候，再创建新的blog.

---
我觉得除了记录github基础知识外，第一步应该记录我是如何创建这个网址的：
1.注册或登录 GitHub
2.创建一个新的仓库，名字格式必须是：your-username.github.io
那我的就是：likai888.github.io

3.编辑**目录结构**文件
```bash
likai888.github.io/
├── _config.yml         <- 网站配置文件
├── index.md            <- 首页内容
├── _posts/             <- 存放你的学习笔记文章（按日期命名）
│   └── 2025-04-01-first-note.md
├── about.md            <- 研究兴趣页
└── assets/             <- 可选，存放图片、附件等
```
4.编辑 **_config.yml** 文件
```bash
title: 豆豆爸学习生信
description: 记录学习过程和错误改正笔记
baseurl: ""
url: "https://likai888.github.io"
theme: minima
plugins:
  - jekyll-feed
```
5. 编辑**index.md** 文件
```bash
---
layout: home
title: 豆豆爸学生信
---

欢迎来到我的博客！  
这里是我记录**生物信息学学习过程**的地方，内容包括学习笔记、常见错误与解决办法等。

点击上方标题或浏览下方的文章列表开始吧～
```
6. 编辑**about.md** 文件
```bash
---
layout: page
title: 我的研究兴趣
permalink: /about/
---

我目前的研究兴趣是：  
📌 **马的基因组组装与注释**

我希望通过系统学习生信分析流程，更深入理解染色体结构、重复序列和物种特异性基因内容。
```
7. 接下来就是创建 **_posts** 文件夹， 然后开始第一篇博客


---

## 🧠 什么是 Git 和 GitHub？

- **Git** 是一个分布式版本控制系统，帮助我们记录每一次修改代码或文档的历史。
- **GitHub** 是一个基于 Git 的代码托管平台，可以远程保存、展示、协作代码项目，还可以搭建博客（如 GitHub Pages）。

---

## 🧰 安装与配置

### 1. 安装 Git

可从 [https://git-scm.com](https://git-scm.com) 下载适合自己系统的版本。

### 2. 配置 Git 账户

```bash
git config --global user.name "你的名字"
git config --global user.email "你的邮箱"
```

---

## 🔑 GitHub 常用术语

| 术语          | 含义 |
|---------------|------|
| Repository    | 仓库，项目的文件夹 |
| Commit        | 一次更改记录 |
| Push / Pull   | 推送 / 拉取代码 |
| Clone         | 克隆整个仓库 |
| Branch        | 分支，不同开发路径 |
| Fork          | 复制别人项目到自己账号下 |
| Pull Request  | 提交修改请求，协作使用 |
| Issues        | 提问、记录问题、建议 |

---

## 🧪 常用操作

### 1. 创建仓库

在 GitHub 网页端点击 `New Repository` 创建新仓库。

### 2. 本地 clone 仓库

```bash
git clone https://github.com/用户名/仓库名.git
```

### 3. 提交更改到 GitHub

```bash
git add .
git commit -m "添加新的博客文章"
git push
```

---

## 🌿 分支管理

### 创建新分支并切换过去

```bash
git checkout -b dev
```

### 查看所有分支

```bash
git branch
```

### 合并分支到主分支

```bash
git checkout main
git merge dev
```

---

## 🤝 与他人协作

### Fork 项目并 Clone 到本地

```bash
git clone https://github.com/你的用户名/对方的项目.git
```

### 发起 Pull Request（PR）

在 GitHub 页面点击 “Pull requests” > “New pull request”，填写说明后提交。

---

## 📚 GitHub Pages 建站

1. 创建仓库 `yourusername.github.io`
2. 上传网页或博客代码（可使用 Jekyll）
3. 等待几分钟访问 `https://yourusername.github.io` 即可上线

---

## 🧼 常用补充命令

```bash
git status       # 查看当前修改状态
git log          # 查看提交历史
git diff         # 查看改动内容
git rm 文件名    # 从 Git 中删除文件
```

---

## 💡 小结

Git 和 GitHub 是现代科研工作不可或缺的工具。掌握它们可以帮助我们：

- 高效地管理代码/笔记版本
- 和他人协同开发脚本
- 公开展示自己的项目
- 用 GitHub Pages 写博客分享

---


