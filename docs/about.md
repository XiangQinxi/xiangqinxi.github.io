# 关于我

你好，我是 **XiangQinxi**。

大概从 2022 年开始，我一直在做同一件事：**让 Python 的桌面界面看起来不像上个时代的产物**。
`tkinter` 是 Python 自带、最轻量的 GUI 方案，但它的默认外观和交互一直很「复古」。
于是我从组件库开始，一路写到了绘制引擎。

## 我在做什么

<div class="grid cards" markdown>

-   :material-palette-outline:{ .lg .middle } **现代化 Tkinter**

    tkfluent 提供 Fluent / WinUI 3 风格的控件；tkdeft 负责底层的矢量绘制；
    tkadw 是更早的一次尝试。这三个项目的共同目标是：让 `tkinter` 项目不用换框架
    也能拥有现代外观。

-   :material-vector-square:{ .lg .middle } **自绘与渲染**

    tkdeft 把绘制引擎抽象成可插拔的一层（Tk 原生 / tksvg / Wand / Skia / Pillow / Cairo），
    同一套控件可以在不同引擎上渲染。这既是性能实验，也是兼容性兜底。

-   :material-web:{ .lg .middle } **Python 也能写 Web**

    Streamlit、NiceGUI 这些小工具是我验证想法的地方：论坛、临时文件交换、
    游戏、视频背景……做完就开源，顺便给 NiceGUI 补了中文文档站。

-   :material-book-open-variant:{ .lg .middle } **写文档**

    每个项目都配了文档站（MkDocs Material），NiceGUI 的中文翻译也在维护。
    代码能跑只是及格线，别人能上手才算完成。

</div>

## 技术栈

| 领域 | 常用技术 |
| :--- | :--- |
| 语言 | Python（主力）、少量 HTML / CSS / JavaScript |
| 桌面 GUI | Tkinter / Tcl-Tk、tkdeft、tkfluent、suzaku |
| 图形绘制 | SVG（`svgwrite`）、Pillow、Wand、Skia、Cairo |
| Web | Streamlit、NiceGUI（FastAPI + Vue）、PyWebIO |
| 文档 | MkDocs Material、GitHub Actions、Netlify |

## 时间线

<div class="timeline" markdown>

- <span class="timeline__date">2022</span> 开始写 Python，个人主页上线
- <span class="timeline__date">2023</span> tkadw `0.4.9`，第一次把 Tkinter 做出 ADW 风格
- <span class="timeline__date">2025</span> tkdeft 立项，tkfluent 发布第一个可用版本
- <span class="timeline__date">2026</span> tkfluent `0.5.0` 重写主题切换；suzaku 与 NiceGUI 相关项目继续推进

</div>

## 联系我

<div class="contact" markdown>

- :fontawesome-brands-github: [@XiangQinxi](https://github.com/XiangQinxi){ target="_blank" rel="noopener" }
- :fontawesome-brands-python: [PyPI · XiangQinxi](https://pypi.org/user/XiangQinxi/){ target="_blank" rel="noopener" }
- :fontawesome-brands-gitlab: [GitLab · XiangQinxi](https://gitlab.com/XiangQinxi){ target="_blank" rel="noopener" }
- :fontawesome-brands-bilibili: [哔哩哔哩](https://space.bilibili.com/471425191){ target="_blank" rel="noopener" }
- :fontawesome-solid-envelope: <xiangqinxi@outlook.com>

</div>

!!! tip "提 Issue 比发邮件更快"
    项目问题优先在对应仓库开 Issue；只有站点本身或合作相关的事，再走邮件。
