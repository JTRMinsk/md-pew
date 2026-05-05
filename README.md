# md-pew

md-pew 是一个轻量的 Markdown 编辑和预览工具，当前以单个本地 HTML 文件运行。

md-pew is a lightweight Markdown editor and previewer that currently runs as a single local HTML file.

打开 `md-pew.html`，拖入 Markdown 文件，就可以在左侧编辑、右侧预览。它不需要安装依赖，也不会把文件发送到任何地方。

Open `md-pew.html`, drag in a Markdown file, edit on the left, and preview on the right. It works without installing dependencies or sending files anywhere.

## 当前功能 / Current Features

- 打开 Markdown 文件，支持拖拽和文件选择器。
- Open Markdown files by drag and drop or file picker.
- 编辑 Markdown，并实时预览。
- Edit Markdown and preview it live.
- 在编辑、分栏和预览视图之间切换。
- Switch between edit, split, and preview views.
- 在浏览器支持时，通过 File System Access API 保存回原文件。
- Save through the browser File System Access API when available.
- 当无法直接写回文件时，下载 Markdown 副本。
- Download a Markdown copy when direct file write access is unavailable.
- 导出当前文档为独立 HTML 文件。
- Export the current document as a standalone HTML file.
- 预览常见 Mermaid `flowchart` 图，并支持 `classDef` 颜色样式。
- Preview common Mermaid `flowchart` diagrams with `classDef` color styles.
- Mermaid 图过大时显示滚动框，并只在需要时提供展开/收起按钮。
- Show scrollable Mermaid diagram frames when needed, with expand/collapse controls only for overflowing diagrams.

## 运行方式 / Run

双击打开：

Double-click:

```text
md-pew.html
```

为了获得更好的保存回原文件体验，建议使用 Chrome 或 Edge。部分浏览器可以预览拖入的文件，但只能下载保存副本。

For best save-back behavior, open it in Chrome or Edge. Some browsers can preview dropped files but only allow downloading a saved copy.

## 项目结构 / Project Shape

```text
md-pew/
  md-pew.html
  README.md
  CHANGELOG.md
  COPYRIGHT
  docs/
    ROADMAP.md
    RELEASE_PROCESS.md
    decisions/
      0001-single-file-first.md
```

## 开发说明 / Development Notes

第一版刻意保持无构建步骤，让应用在核心体验还在打磨时依然便携、容易分享。

The first version intentionally has no build step. That keeps the app portable while the core UX is still being shaped.

版本历史记录在 `CHANGELOG.md`。每次迭代完成前，都要记录版本号、日期、中英双语改动内容和验证结果。

Version history is stored in `CHANGELOG.md`. Every iteration should record the version number, date, bilingual changes, and verification before it is considered done.

README 和 CHANGELOG 默认使用中英双语，中文在前，英文在后。

README and CHANGELOG entries are bilingual by default, with Chinese first and English second.

后续如果安装 Rust/Cargo，并且需要 Windows 和 macOS 原生应用打包，可以把项目迁移到 Tauri。

Later, this project can move to Tauri when Rust/Cargo is installed and we want native app packaging for Windows and macOS.

## 作者 / Author

Salim Sehng

## 版权 / Copyright

Copyright (c) 2026 Salim Sehng. All rights reserved.

目前尚未选择开源许可证。

No open-source license has been selected yet.
