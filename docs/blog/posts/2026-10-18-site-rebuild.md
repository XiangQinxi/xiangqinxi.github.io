---
date: 2026-10-18
categories:
  - 站点
  - MkDocs
---

# 把这个站点推倒重来

这个仓库从 2022 年就在了，中间零星改过几次，但一直是「能打开就行」的状态。
最近打开 `xiangqinxi.github.io`，看到的却只有一行 **Site not found** ——
配置和部署其实早就坏了，只是一直没人发现。

一张坏掉的页面，比没有页面更糟。所以这次把它整个重做了一遍。

<!-- more -->

## 问题出在哪

排查下来是三件事叠在一起：

1. **`mkdocs.yml` 里有两个 `plugins:` 键。** YAML 后键覆盖前键，第一个里的
   `mkdocstrings`、`meta`、`offline` 全部静默失效。改配置改了半年都没生效，原因在这儿。
2. **部署工作流的 YAML 是坏的。** 文件里写的是

    ```yaml
    on:
      push:
        分支: ["main"]
    ```

    `分支` 不是 GitHub Actions 认的键，整个工作流从未触发成功过。

3. **Pages 的来源被改成了 GitHub Actions，但没有一次成功的 deployment。**
   所以线上就只剩 404。

另外 `site/` 构建产物被提交进了仓库，`requirements.txt` 没固定版本，
两个工作流互相打架 —— 一个走 `gh-deploy` 推 `gh-pages` 分支，另一个走
`upload-pages-artifact`，总有一个在覆盖另一个。

## 新结构

```text
.
├── .github/workflows/
│   ├── pages.yml        # push 到 main：构建 + 部署 Pages
│   └── ci.yml           # PR：只构建检查
├── docs/
│   ├── index.md         # 首页
│   ├── projects.md      # 项目集
│   ├── changelog.md     # 更新日志
│   ├── blog/            # 博客（Material blog 插件）
│   ├── about.md         # 关于
│   └── stylesheets/extra.css
├── mkdocs.yml
└── requirements.txt     # 固定版本
```

内容上补了项目集、更新日志和博客；样式上加了 hero 区、数据条、卡片悬停效果和
深色模式的单独配色。整体仍然是 Material for MkDocs —— 和 tkfluent、tkdeft 的文档站
保持同一套工具链，维护成本最低。

## 部署

部署改成官方推荐的两段式：

- `build`：`actions/checkout`（`fetch-depth: 0`，给 `git-revision-date-localized` 用）
  → `setup-python` → `pip install -r requirements.txt` → `mkdocs build --strict`
  → `upload-pages-artifact`
- `deploy`：`deploy-pages`，只在 `main` 分支执行

`--strict` 很关键：任何死链、警告都会让构建失败，而不是默默发一个坏页面出去。

## 下一步

- 把几篇拖了很久的 tkfluent 实现笔记写出来
- 给项目集加上真实的发布状态徽章
- 等 `suzaku` 稳定一点，单独做个文档站

如果你也在维护一个几年没动的个人站，去 Actions 页面看一眼最近一次运行为什么是红的吧 ——
大概率不是你想的那个原因。
