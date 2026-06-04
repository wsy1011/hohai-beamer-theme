# Hohai University Beamer Theme

[中文](#中文说明) | [English](#english)

## 中文说明

这是一个面向河海大学风格演示文稿的 Beamer 主题项目。项目在 `collegebeamer` 风格组织基础上增加了 `hhu` 主题选项，并提供了可直接用 XeLaTeX 编译的示例文档。

### 主要特性

- 河海大学蓝白视觉风格的 Beamer 模板。
- 封面页、章节页、普通内容页和 Q&A 页的统一版式。
- 正文字体使用 Arial；数学公式保持 LaTeX 默认数学字体。
- 内置河海大学校徽、英文校名文字图、PPT 图标 SVG 素材和素材来源说明。

### 文件结构

```text
.
|-- collegebeamer.sty
|-- example.tex
|-- README.md
|-- LICENSE
|-- NOTICE.md
`-- assets/
    |-- hhu/
    |   |-- color-logo.png
    |   |-- trans-logo.png
    |   |-- hhu-wordmark.png
    |   |-- hhu-emblem.png
    |   `-- background.png
    |-- official-pptx-icons/
    |   |-- manifest.csv
    |   |-- manifest.json
    |   `-- slide-*/
    `-- source-vector/
        `-- hhu-emblem.ai
```

### 编译方式

请使用 XeLaTeX：

```powershell
xelatex -interaction=nonstopmode example.tex
xelatex -interaction=nonstopmode example.tex
```

如果安装了 `latexmk`，也可以使用：

```powershell
latexmk -xelatex -interaction=nonstopmode example.tex
```

### 使用方式

在你的 Beamer 文档中加载主题：

```latex
\documentclass[aspectratio=169,10pt]{beamer}
\usepackage[hhu,en]{collegebeamer}
```

将 `collegebeamer.sty`、`assets/hhu/` 和你的 `.tex` 文件放在同一项目目录下即可。

### 素材来源与授权边界

本项目中整理的河海大学视觉素材来源于官方公开材料：

- 河海大学视觉形象页面：<https://www.hhu.edu.cn/236/list.htm>
- 河海大学官方 PPT 模板和素材：<https://mp.weixin.qq.com/s/GmgyDONKJUlGBilQb0WJAg>

代码部分按 `LICENSE` 开源。河海大学名称、校徽、logo、PPT 图标和相关视觉资产不因本仓库而被重新授权；发布、再分发或公开使用这些视觉资产前，请确认你具备相应使用权限。详情见 `NOTICE.md`。

## English

This repository provides a Hohai University styled Beamer theme. It extends the `collegebeamer` style organization with an `hhu` theme option and includes a XeLaTeX-ready example document.

### Features

- Blue-and-white Beamer theme inspired by Hohai University's visual identity.
- Consistent layouts for title slides, section slides, regular content slides, and Q&A slides.
- Arial for presentation text while keeping LaTeX's default math fonts for formulas.
- Organized Hohai University emblem, wordmark, PPT icon SVG assets, and source documentation.

### Repository Layout

```text
.
|-- collegebeamer.sty
|-- example.tex
|-- README.md
|-- LICENSE
|-- NOTICE.md
`-- assets/
    |-- hhu/
    |   |-- color-logo.png
    |   |-- trans-logo.png
    |   |-- hhu-wordmark.png
    |   |-- hhu-emblem.png
    |   `-- background.png
    |-- official-pptx-icons/
    |   |-- manifest.csv
    |   |-- manifest.json
    |   `-- slide-*/
    `-- source-vector/
        `-- hhu-emblem.ai
```

### Compile

Use XeLaTeX:

```powershell
xelatex -interaction=nonstopmode example.tex
xelatex -interaction=nonstopmode example.tex
```

Or, with `latexmk`:

```powershell
latexmk -xelatex -interaction=nonstopmode example.tex
```

### Usage

Load the theme in your Beamer document:

```latex
\documentclass[aspectratio=169,10pt]{beamer}
\usepackage[hhu,en]{collegebeamer}
```

Place `collegebeamer.sty`, `assets/hhu/`, and your `.tex` file in the same project directory.

### Asset Sources and License Boundary

The Hohai University visual assets organized in this repository come from official public sources:

- Hohai University visual identity page: <https://www.hhu.edu.cn/236/list.htm>
- Official Hohai University PPT template and materials: <https://mp.weixin.qq.com/s/GmgyDONKJUlGBilQb0WJAg>

The source code is licensed under `LICENSE`. Hohai University names, marks, emblems, logos, PPT icons, and related visual assets are not relicensed by this repository. Confirm your permission before publishing, redistributing, or publicly using those assets. See `NOTICE.md` for details.
