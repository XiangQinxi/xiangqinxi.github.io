---
hide:
  - navigation
  - toc
---

<div class="hero">
  <div class="hero__logo">
    <img src="assets/logo.svg" alt="XiangQinxi 的 Logo">
  </div>
  <div class="hero__body">
    <p class="hero__eyebrow">Hello, world 👋</p>
    <h1 class="hero__title">XiangQinxi</h1>
    <p class="hero__desc">
      喜欢把 <code>tkinter</code> 折腾成现代界面的 Python 开发者。<br>
      维护 <strong>tkfluent</strong>、<strong>tkdeft</strong>、<strong>suzaku</strong> 等开源项目，
      也写一点 Streamlit 小工具和中文文档。
    </p>
    <p class="hero__actions">
      <a class="md-button md-button--primary" href="projects/">浏览项目集</a>
      <a class="md-button" href="https://github.com/XiangQinxi" target="_blank" rel="noopener">GitHub</a>
      <a class="md-button" href="https://pypi.org/user/XiangQinxi/" target="_blank" rel="noopener">PyPI</a>
    </p>
  </div>
</div>

<div class="stats">
  <div class="stat"><span class="stat__num">6</span><span class="stat__label">PyPI 包</span></div>
  <div class="stat"><span class="stat__num">30+</span><span class="stat__label">公开仓库</span></div>
  <div class="stat"><span class="stat__num">2022</span><span class="stat__label">开始开源</span></div>
  <div class="stat"><span class="stat__num">4</span><span class="stat__label">年持续折腾</span></div>
</div>

## 精选项目

<div class="grid cards" markdown>

-   :material-palette-outline:{ .lg .middle } **tkfluent**

    ---

    Fluent / WinUI 3 风格的 Tkinter 组件库，换肤、动画、可切换绘制引擎。

    [:octicons-arrow-right-24: 文档](https://tkfluent.netlify.app/){ target="_blank" rel="noopener" }
    · [:octicons-package-24: PyPI](https://pypi.org/project/tkfluent/){ target="_blank" rel="noopener" }

-   :material-vector-square:{ .lg .middle } **tkdeft**

    ---

    tkfluent 的底座：把矢量绘制变成 Tkinter 控件的绘制引擎层。

    [:octicons-arrow-right-24: 文档](https://tkdeft.netlify.app/){ target="_blank" rel="noopener" }
    · [:octicons-package-24: PyPI](https://pypi.org/project/tkdeft/){ target="_blank" rel="noopener" }

-   :material-rocket-launch-outline:{ .lg .middle } **suzaku**

    ---

    另一套从零写的 Python GUI 库，外观与性能都想要比 tkinter 更好。

    [:octicons-mark-github-16: GitHub](https://github.com/XiangQinxi/suzaku){ target="_blank" rel="noopener" }
    · [:octicons-package-24: PyPI](https://pypi.org/project/suzaku/){ target="_blank" rel="noopener" }

-   :material-web:{ .lg .middle } **nicegui-shadcn**

    ---

    给 NiceGUI 用的 shadcn/ui 组件集，自带编译好的 Tailwind 主题。

    [:octicons-arrow-right-24: 文档](https://github.com/XiangQinxi/nicegui-shadcn/tree/master/docs){ target="_blank" rel="noopener" }
    · [:octicons-package-24: PyPI](https://pypi.org/project/nicegui-shadcn/){ target="_blank" rel="noopener" }

-   :material-history:{ .lg .middle } **tkadw**

    ---

    早期的 Tkinter 扩展组件库（Windows ADW 风格），tkfluent 的前身之一。

    [:octicons-arrow-right-24: 文档](https://tkadwite.netlify.app/){ target="_blank" rel="noopener" }
    · [:octicons-package-24: PyPI](https://pypi.org/project/tkadw/){ target="_blank" rel="noopener" }

-   :material-video:{ .lg .middle } **streamlit-video-background**

    ---

    一行代码给 Streamlit 页面加上全屏循环视频背景。

    [:octicons-package-24: PyPI](https://pypi.org/project/streamlit-video-background/){ target="_blank" rel="noopener" }
    · [:octicons-mark-github-16: 源码](https://github.com/XiangQinxi/streamlit-video-background){ target="_blank" rel="noopener" }

</div>

[:octicons-arrow-right-24: 查看全部项目](projects.md){ .md-button }

## 最近动态

<div class="timeline" markdown>

- <span class="timeline__date">2026-10-18</span> 站点用 MkDocs Material 重做，改由 GitHub Actions 自动构建部署
- <span class="timeline__date">2026-09-24</span> tkfluent `0.5.0`：把主题切换重写成一条统一时间轴
- <span class="timeline__date">2026-09-16</span> tkdeft `0.3.0` / tkfluent `0.3.0`：补齐对外接口
- <span class="timeline__date">2026-09-12</span> tkdeft `0.2.0`：可插拔绘制引擎层

</div>

[:octicons-history-16: 完整更新日志](changelog.md) ·
[:octicons-pencil-16: 博客文章](blog/index.md)

## 关于这个站点

这里记录我在 Python 桌面 GUI、图形绘制和 Web 小工具上折腾出来的东西。
文档由 [MkDocs](https://www.mkdocs.org/) + [Material for MkDocs](https://squidfunk.github.io/mkdocs-material/) 构建，
推送到 `main` 后由 GitHub Actions 自动发布到 GitHub Pages。

想聊点什么？欢迎从 [关于页](about.md) 找我。
