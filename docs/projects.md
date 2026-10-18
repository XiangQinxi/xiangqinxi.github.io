---
hide:
  - toc
---

# 项目集

按主题整理我比较常维护的开源项目。完整列表见
[GitHub 主页](https://github.com/XiangQinxi?tab=repositories){ target="_blank" rel="noopener" }，
可安装的包见 [PyPI 主页](https://pypi.org/user/XiangQinxi/){ target="_blank" rel="noopener" }。

## 桌面 GUI

<div class="grid cards" markdown>

-   :material-palette-outline:{ .lg .middle } **tkfluent** `v0.5.0`

    ---

    Fluent / WinUI 3 风格的 Tkinter 组件库。59 个控件、多套可插拔绘制引擎
    （tksvg / wand / skia / pillow / cairo），0.5 起主题切换统一成一条时间轴，
    换肤从数秒降到约 30 ms。

    [:octicons-arrow-right-24: 文档](https://tkfluent.netlify.app/){ target="_blank" rel="noopener" }
    · [:octicons-package-24: PyPI](https://pypi.org/project/tkfluent/){ target="_blank" rel="noopener" }
    · [:octicons-mark-github-16: 源码](https://github.com/XiangQinxi/tkfluent){ target="_blank" rel="noopener" }

-   :material-vector-square:{ .lg .middle } **tkdeft** `v0.3.0`

    ---

    tkfluent 的绘制底座：把 SVG / 位图矢量绘图封装成标准的 Tkinter 控件，
    并提供可插拔的绘制引擎层，让「换引擎不换代码」成为可能。

    [:octicons-arrow-right-24: 文档](https://tkdeft.netlify.app/){ target="_blank" rel="noopener" }
    · [:octicons-package-24: PyPI](https://pypi.org/project/tkdeft/){ target="_blank" rel="noopener" }
    · [:octicons-mark-github-16: 源码](https://github.com/XiangQinxi/tkdeft){ target="_blank" rel="noopener" }

-   :material-rocket-launch-outline:{ .lg .middle } **suzaku** `v0.2.1`

    ---

    从零写的 Python GUI 库，目标是外观和性能都超过 tkinter，纯 Python 实现。

    [:octicons-package-24: PyPI](https://pypi.org/project/suzaku/){ target="_blank" rel="noopener" }
    · [:octicons-mark-github-16: 源码](https://github.com/XiangQinxi/suzaku){ target="_blank" rel="noopener" }

-   :material-history:{ .lg .middle } **tkadw**

    ---

    早期的 Tkinter 扩展组件库（Windows ADW 风格），tkfluent 的「前身」之一，
    保留下来给老项目用。

    [:octicons-arrow-right-24: 文档](https://tkadwite.netlify.app/){ target="_blank" rel="noopener" }
    · [:octicons-package-24: PyPI](https://pypi.org/project/tkadw/){ target="_blank" rel="noopener" }

-   :material-window-maximize:{ .lg .middle } **tktitlebar**

    ---

    给 Windows 上的 tkinter 窗口换一个自定义标题栏，还可以把小组件直接放进标题栏。

    [:octicons-mark-github-16: 源码](https://github.com/XiangQinxi/tktitlebar){ target="_blank" rel="noopener" }

-   :material-translate:{ .lg .middle } **ttkbootstrap-ttkcreator--**

    ---

    [ttkbootstrap](https://github.com/israel-dryer/ttkbootstrap) 可视化样式编辑器
    ttkcreator 的汉化版，方便中文用户直接上手。

    [:octicons-mark-github-16: 源码](https://github.com/XiangQinxi/ttkbootstrap-ttkcreator--){ target="_blank" rel="noopener" }

</div>

## Web 与 Streamlit

<div class="grid cards" markdown>

-   :material-video:{ .lg .middle } **streamlit-video-background** `v0.2.0`

    ---

    一行代码给 Streamlit 页面加上全屏循环视频背景，自动处理覆盖层与内容层级。

    [:octicons-package-24: PyPI](https://pypi.org/project/streamlit-video-background/){ target="_blank" rel="noopener" }
    · [:octicons-mark-github-16: 源码](https://github.com/XiangQinxi/streamlit-video-background){ target="_blank" rel="noopener" }

-   :material-forum-outline:{ .lg .middle } **freelake**

    ---

    用 Streamlit + peewee + SQLite 写的完整论坛：注册登录、发帖评论、点赞收藏、
    举报审核都有。[在线体验](https://freelake.streamlit.app/){ target="_blank" rel="noopener" }

    [:octicons-mark-github-16: 源码](https://github.com/XiangQinxi/freelake){ target="_blank" rel="noopener" }

-   :material-swap-horizontal:{ .lg .middle } **SwiftZ**

    ---

    临时文件交换站：上传拿到取件码，另一端凭码下载，适合临时传文件。
    [在线体验](https://swiftz.streamlit.app/){ target="_blank" rel="noopener" }

    [:octicons-mark-github-16: 源码](https://github.com/XiangQinxi/SwiftZ){ target="_blank" rel="noopener" }

-   :material-incognito:{ .lg .middle } **who_is_spy**

    ---

    「谁是卧底」多人 Web 版：词库管理、多人同时在线、AI 辅助分析玩家描述与投票。

    [:octicons-mark-github-16: 源码](https://github.com/XiangQinxi/who_is_spy){ target="_blank" rel="noopener" }

</div>

## 文档与学习资料

<div class="grid cards" markdown>

-   :material-book-open-variant:{ .lg .middle } **NiceGUI-docs**

    ---

    [nicegui.cn](https://nicegui.cn/){ target="_blank" rel="noopener" } 的源码：
    把 NiceGUI 官方英文文档翻译成简体中文，配合
    [nicegui-shadcn](https://github.com/XiangQinxi/nicegui-shadcn){ target="_blank" rel="noopener" }
    一起看更完整。

    [:octicons-mark-github-16: 仓库](https://github.com/XiangQinxi/NiceGUI-docs){ target="_blank" rel="noopener" }

-   :material-file-document-multiple:{ .lg .middle } **suzaku-docs**

    ---

    suzaku 的文档站源码（HTML + MkDocs 混合）。

    [:octicons-mark-github-16: 仓库](https://github.com/XiangQinxi/suzaku-docs){ target="_blank" rel="noopener" }

-   :material-application-brackets:{ .lg .middle } **Gibox**

    ---

    GTK 界面的「盒子」：把常用 GTK 布局和组件组合封装成即插即用模块。

    [:octicons-mark-github-16: 仓库](https://github.com/XiangQinxi/Gibox){ target="_blank" rel="noopener" }

-   :material-web:{ .lg .middle } **本站**

    ---

    MkDocs Material 构建，GitHub Actions 自动部署。源码就在
    [xiangqinxi.github.io](https://github.com/XiangQinxi/xiangqinxi.github.io){ target="_blank" rel="noopener" }。

    [:octicons-arrow-right-24: 仓库](https://github.com/XiangQinxi/xiangqinxi.github.io){ target="_blank" rel="noopener" }

</div>

## 其它

- [QRCreator](https://github.com/XiangQinxi/QRCreator){ target="_blank" rel="noopener" }：二维码生成小工具
- [PictureSelector](https://github.com/XiangQinxi/PictureSelector){ target="_blank" rel="noopener" }：图片选择/预览小组件
- [Yes-Steve-Model-Repo](https://github.com/XiangQinxi/Yes-Steve-Model-Repo){ target="_blank" rel="noopener" }：学习用 fork
- [win32mica](https://github.com/XiangQinxi/win32mica){ target="_blank" rel="noopener" }：上游 fork

!!! note "关于 fork"
    仓库列表里的 `streamlit-shadcn-ui`、`win32mica`、`Yes-Steve-Model-Repo`
    等是上游项目的 fork，作者是原项目维护者，这里不重复介绍。
