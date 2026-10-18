---
hide:
  - toc
---

# 更新日志

站点本身与主要项目的版本更新都记在这里。每个 PyPI 包也能在包页的
[Release history](https://pypi.org/user/XiangQinxi/){ target="_blank" rel="noopener" } 里查到完整版本。

<div class="timeline" markdown>

## 2026

- <span class="timeline__date">2026-10-18</span>

    **本站 · 用 MkDocs Material 重做**

    旧的 `mkdocs.yml` 有重复的 `plugins` 键、工作流使用了非法的 YAML 键，部署一直是坏的。
    这次补齐 `site_url`、博客/更新日期插件、暗色模式与自定义样式，并把部署改成官方的
    `deploy-pages` 流程。

    [GitHub Actions 工作流](https://github.com/XiangQinxi/xiangqinxi.github.io/tree/main/.github/workflows){ target="_blank" rel="noopener" }

- <span class="timeline__date">2026-10-11</span>

    **nicegui-shadcn `0.1.6`**

    NiceGUI 的 shadcn/ui 组件集，补齐组件与编译好的 Tailwind 主题。
    [PyPI](https://pypi.org/project/nicegui-shadcn/){ target="_blank" rel="noopener" } ·
    [文档](https://github.com/XiangQinxi/nicegui-shadcn/tree/master/docs){ target="_blank" rel="noopener" }

- <span class="timeline__date">2026-09-24</span>

    **tkfluent `0.5.0`**

    主题过渡重写：所有控件的换肤合并到同一条时间轴上，59 个控件整体切换从
    2.8 ~ 4.0 s 降到约 30 ms，而且过渡发生在同一帧里，不再逐个闪。
    [更新说明](https://github.com/XiangQinxi/tkfluent/releases){ target="_blank" rel="noopener" } ·
    [PyPI](https://pypi.org/project/tkfluent/){ target="_blank" rel="noopener" }

- <span class="timeline__date">2026-09-16</span>

    **tkdeft `0.3.0` · tkfluent `0.3.0`**

    绘制引擎层稳定下来：`CairoEngine`、`WandEngine`、`TkSVGEngine` 可以互换，
    tkfluent 跟着打磨了一批控件。

- <span class="timeline__date">2026-09-12</span>

    **tkdeft `0.2.0` · tkfluent `0.2.0`**

    tkdeft 引入可插拔绘制引擎；tkfluent 开始把所有控件迁到 tkdeft 上。

- <span class="timeline__date">2026-08-23</span>

    **streamlit-video-background `0.2.0`**

    支持自定义遮罩、静音与循环参数。
    [PyPI](https://pypi.org/project/streamlit-video-background/){ target="_blank" rel="noopener" }

## 2025

- <span class="timeline__date">2025-12-21</span>

    **suzaku `0.2.1`**

    纯 Python 的新 GUI 库，修掉高 DPI 下的布局问题。

- <span class="timeline__date">2025-07-06</span>

    **tkfluent `0.1.6`**

    第一个能装进生产项目的版本：基础控件、深色模式、`tkinter` 无缝替换。

- <span class="timeline__date">2025-06-26</span>

    **tkdeft `0.1.0`**

    把 `svgwrite` 绘制的矢量图变成真正的 Tkinter 控件。

- <span class="timeline__date">2025-06-22</span>

    **tkfluent `0.1.0`**

    首次发布。

## 2023

- <span class="timeline__date">2023-12-23</span>

    **tkadw `0.4.9`**

    Windows ADW 风格的 Tkinter 扩展库的最后一个版本，之后精力转向 tkdeft / tkfluent。

## 2022

- <span class="timeline__date">2022</span>

    **本站上线**

    最早只是一个手写 HTML 的个人主页。

</div>
