# xiangqinxi.github.io

[![pages](https://github.com/XiangQinxi/xiangqinxi.github.io/actions/workflows/pages.yml/badge.svg)](https://github.com/XiangQinxi/xiangqinxi.github.io/actions/workflows/pages.yml)
[![site](https://img.shields.io/badge/site-xiangqinxi.github.io-indigo)](https://xiangqinxi.github.io/)
[![docs](https://img.shields.io/badge/docs-MkDocs%20Material-blueviolet)](https://squidfunk.github.io/mkdocs-material/)

XiangQinxi 的个人站点：用来归档开源项目、更新日志和折腾笔记。

- 站点：<https://xiangqinxi.github.io/>
- 技术栈：MkDocs + Material for MkDocs
- 部署：推送 `main` 后由 GitHub Actions 自动构建并发布到 GitHub Pages

## 目录结构

```text
.
├── .github/
│   ├── dependabot.yml          # 依赖与 Actions 自动更新
│   └── workflows/
│       ├── pages.yml           # main：构建 + 部署到 Pages
│       └── ci.yml              # PR：只构建检查（--strict）
├── docs/
│   ├── index.md                # 首页（hero / 数据条 / 精选项目）
│   ├── projects.md             # 项目集
│   ├── changelog.md            # 更新日志
│   ├── about.md                # 关于
│   ├── blog/
│   │   └── posts/              # 博客文章（文件名 yyyy-mm-dd-slug.md）
│   ├── assets/                 # logo / favicon
│   └── stylesheets/extra.css   # 自定义样式
├── overrides/
│   └── 404.html                # 自定义 404 页（中文文案）
├── mkdocs.yml
└── requirements.txt            # 固定版本的构建依赖
```

## 本地开发

```bash
# 1. 创建虚拟环境
python -m venv .venv
source .venv/bin/activate        # Windows: .venv\Scripts\activate

# 2. 安装依赖
pip install -r requirements.txt

# 3. 本地预览（http://127.0.0.1:8000）
mkdocs serve

# 4. 发布前检查：死链、废弃语法都会报错
mkdocs build --strict
```

## 部署说明

工作流已经写好，但**仓库设置需要手动确认一次**：

1. 打开 `Settings → Pages`
2. `Build and deployment → Source` 选择 **GitHub Actions**（不要选 Deploy from a branch）
3. 推送到 `main`，或在 `Actions` 页面手动运行 `pages` 工作流
4. 等 `Deploy to GitHub Pages` 变绿后访问 <https://xiangqinxi.github.io/>

> 如果这个仓库还保留着旧的 `gh-pages` 分支，确认新流程可用后可以删除。

## 内容维护

- **新增项目**：在 `docs/projects.md` 对应的分类里加一张卡片，版本号与链接从 PyPI / GitHub 抄过来
- **新增日志**：在 `docs/changelog.md` 的时间线里追加一条
- **写博客**：在 `docs/blog/posts/` 新建 `yyyy-mm-dd-slug.md`，开头写 front matter：

  ```yaml
  ---
  date: 2026-10-18
  categories:
    - 站点
  ---
  ```

- **改样式**：尽量用 Material 暴露的 CSS 变量（`--md-primary-fg-color` 等），少写硬编码颜色，深色模式才不跑偏

## License

站点文字内容归 XiangQinxi 所有；主题与配置代码可随意参考。
