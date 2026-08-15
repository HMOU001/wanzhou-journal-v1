# 晚舟手记（第一版 · 纸上杂志）

「晚舟手记」个人博客的第一版 —— 纸上杂志风格（编辑人文）。暖纸底、宋体展示、首字下沉、规矩线与目录点线，一套前数字时代的印刷语言。

## 技术栈

- [Astro](https://astro.build) 4.x（静态生成）
- 内容集合（`src/content/posts/`）管理文章
- 无运行时框架、无统计脚本、无评论

## 本地开发

```bash
npm install
npm run dev        # http://localhost:4321
npm run build      # 输出到 dist/
npm run preview    # 预览构建产物
```

## 写作

在 `src/content/posts/` 新增 Markdown，frontmatter 格式：

```yaml
---
title: 文章标题
date: 2026-08-02
tag: 工程笔记
excerpt: 摘要
minutes: 6
---
```

## 结构

- `src/pages/` —— 路由页面（首页 / 文章 / 专题 / 关于 / 订阅 / RSS）
- `src/layouts/Base.astro` —— 全站布局
- `src/styles/global.css` —— 设计系统（变量、排版、响应式）
