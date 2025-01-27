# CentriForce's Blog

基于[🍥Fuwari]()静态博客模板的个人博客。

> README 版本：`2024-09-10`

![Preview Image](https://raw.githubusercontent.com/saicaca/resource/main/fuwari/home.png)

## ✨ 功能特性

- [x] 基于 Astro 和 Tailwind CSS 开发
- [x] 流畅的动画和页面过渡
- [x] 亮色 / 暗色模式
- [x] 自定义主题色和横幅图片
- [x] 响应式设计
- [ ] 评论
- [x] 搜索
- [ ] 文内目录

## 🚀 使用方法

1. 将仓库克隆至本地 `$ git clone https://github.com/CentriForce/CentriForce.github.io.git`
2. 编辑配置文件 `src/config.ts` 来自定义博客
3. 执行 `pnpm new-post <filename>` 创建新 `markdown` 文章，并在 `src/content/posts/` 目录中编辑
4. 保存并 `$ git sync` 或 `$ git push`，github会运行自动任务来部署博客

## 📄 文章头格式

```yaml
---
# 文章标题
title: My First Blog Post
# 发布时间
published: 2023-09-09
# 文章简介
description: This is the first post of my new Astro blog.
# 封面图片
image: ./cover.jpg
# 文章标签
tags: [Foo, Bar]
# 文章分类
category: Front-end
# 是否为草稿（草稿在上传后不会进行部署显示）
draft: false
# 语言（仅当文章语言与 `config.ts` 中的网站语言不同时需要设置）
lang: zh_CN
---
```

## 🧞 指令

下列指令均需要在项目根目录执行：

| Command                          | Action                                 |
| :------------------------------- | :------------------------------------- |
| `pnpm install && pnpm add sharp` | 安装依赖                               |
| `pnpm dev`                       | 在 `localhost:4321` 启动本地开发服务器 |
| `pnpm build`                     | 构建网站至 `./dist/`                   |
| `pnpm preview`                   | 本地预览已构建的网站                   |
| `pnpm new-post <filename>`       | 创建新文章                             |
| `pnpm astro ...`                 | 执行 `astro add`, `astro check` 等指令 |
| `pnpm astro --help`              | 显示 Astro CLI 帮助                    |

## 📝 备注

由于添加了 `.gitignore` ，在本地构建网站并预览的文件不会上传到github中。