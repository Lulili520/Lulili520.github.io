# Lu Blog

Lu 的个人技术博客，使用 Jekyll 构建并发布到 GitHub Pages：

- 站点：https://lulili520.github.io
- 仓库：https://github.com/Lulili520/Lulili520.github.io

## 本地运行

需要 Ruby 3.3、Bundler 和 Node.js。

```bash
bundle install
npm install
npm run assets
npm run serve
```

访问 `http://127.0.0.1:4000`。仅修改文章或页面时，不需要重复执行 `npm run assets`。

## 写文章

在 `_posts` 中新增 `YYYY-MM-DD-slug.md` 文件，并添加 Front Matter：

```yaml
---
layout: post
title: "文章标题"
subtitle: "可选副标题"
date: 2026-08-25 12:00:00 +0800
author: Lu
header-img: img/post-bg-desk.jpg
catalog: true
tags:
  - 示例标签
---
```

## 验证

```bash
npm test
```

该命令会执行完整 Jekyll 构建，输出位于 `_site`。

## 发布

推送到 `master` 后，仓库内的 GitHub Actions 工作流会构建并部署站点。首次使用时，请在仓库的 **Settings → Pages → Build and deployment → Source** 中选择 **GitHub Actions**。

## 致谢

页面样式源自 [Hux Blog](https://github.com/Huxpro/huxpro.github.io) 与 [BY Blog](https://github.com/qiubaiying/qiubaiying.github.io)，项目代码按 [MIT License](LICENSE) 使用。
