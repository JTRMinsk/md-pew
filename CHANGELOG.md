# Changelog / 更新日志

This file is the source of truth for md-pew version history. Every iteration should add a bilingual entry with:

本文件是 md-pew 版本历史的唯一记录。每次迭代都要新增一条中英双语记录，包含：

- Version number / 版本号
- Release date / 发布日期
- User-facing changes / 用户可见改动
- Important implementation notes / 重要实现说明
- Verification performed / 已执行的验证

## Entry Template / 条目模板

```text
## x.y.z - YYYY-MM-DD

### 中文

- 新增：...
- 修改：...
- 修复：...
- 验证：...

### English

- Added: ...
- Changed: ...
- Fixed: ...
- Verified: ...
```

## 0.1.5 - 2026-05-05

### 中文

- 修改：将 `README.md` 改为中英双语，默认中文在前、英文在后。
- 修改：补充 README 中的当前功能说明，让 Mermaid 预览、颜色样式和展开/收起能力也被记录。
- 修改：同步更新发布流程文档，要求 README 和 CHANGELOG 都保持双语规则。
- 验证：检查 `README.md`、`CHANGELOG.md` 和发布流程文档内容。

### English

- Changed: Converted `README.md` to a bilingual format, with Chinese first and English second.
- Changed: Updated the README feature list to include Mermaid preview, color styles, and expand/collapse behavior.
- Changed: Updated the release process to keep both README and CHANGELOG bilingual.
- Verified: Reviewed `README.md`, `CHANGELOG.md`, and the release process documentation.

## 0.1.4 - 2026-05-05

### 中文

- 修改：将更新日志规则改为中英双语，默认中文在前、英文在后。
- 修改：把现有版本记录补成中英双语格式，避免后续格式不一致。
- 修改：同步更新发布流程文档，要求未来每次迭代都记录双语 changelog。
- 验证：检查 `CHANGELOG.md` 和发布流程文档内容。

### English

- Changed: Made changelog entries bilingual, with Chinese first and English second.
- Changed: Converted existing version entries to the bilingual format for consistency.
- Changed: Updated the release process to require bilingual changelog entries for future iterations.
- Verified: Reviewed `CHANGELOG.md` and the release process documentation.

## 0.1.3 - 2026-05-05

### 中文

- 新增：为带内部滚动条的 Mermaid 图增加展开/收起按钮。
- 修改：适合当前显示框的 Mermaid 图不显示展开按钮。
- 修改：展开后的 Mermaid 图会取消宽度和高度上限，让显示框可以扩展到完整图形。
- 修改：导出的 HTML 也保留同样的展开/收起能力。
- 验证：检查 JavaScript 语法，并确认 Mermaid 输出包含按钮，同时保留 SVG 渲染和 class 颜色。

### English

- Added: An expand/collapse toggle for Mermaid diagrams that have internal scrollbars.
- Changed: Kept the toggle hidden for diagrams that fit inside their display frame.
- Changed: Expanded Mermaid diagrams remove width and height caps so the display frame can grow to show the full diagram.
- Changed: Applied the same expand/collapse behavior to exported HTML.
- Verified: Checked JavaScript syntax and confirmed Mermaid output includes the toggle button while retaining SVG rendering and class colors.

## 0.1.2 - 2026-05-05

### 中文

- 修改：Mermaid 图改为按自然 SVG 尺寸显示，不再总是撑满整个预览宽度。
- 修改：收紧 Mermaid 流程图的间距、节点尺寸和字体尺寸，让图更轻巧，同时保持标签可读。
- 新增：为 Mermaid 图设置舒适的最大宽度和最大高度，让大图限制在自己的显示框内滚动。
- 修改：导出的 HTML 使用同样的 Mermaid 尺寸规则。
- 验证：检查 JavaScript 语法，并测量用户报告的 Mermaid 样例输出，确认它是内在 SVG 尺寸而不是强制全宽渲染。

### English

- Changed: Mermaid diagrams render at their natural SVG size instead of always filling the full preview width.
- Changed: Reduced Mermaid flowchart spacing, node size, and text size to make diagrams feel lighter while keeping labels readable.
- Added: A comfortable maximum diagram width and height so large diagrams stay contained and scroll inside their own frame.
- Changed: Applied the same Mermaid sizing rules to exported HTML.
- Verified: Checked JavaScript syntax and measured the reported Mermaid sample output as an intrinsic SVG instead of a forced full-width render.

## 0.1.1 - 2026-05-05

### 中文

- 新增：支持常见 `flowchart TD/LR` Mermaid 流程图预览。
- 新增：支持 Mermaid `classDef` 颜色样式，包括 `fill`、`stroke` 和文字 `color`。
- 新增：支持 Mermaid 流程图中的带标签箭头和虚线箭头。
- 修改：Mermaid 渲染保持自包含，让 `md-pew.html` 仍然可以离线运行，不依赖 CDN 或 npm。
- 验证：检查 JavaScript 语法，并把用户报告的 Mermaid 样例渲染为带预期 class 颜色的 SVG。

### English

- Added: Mermaid flowchart preview support for common `flowchart TD/LR` diagrams.
- Added: Support for Mermaid `classDef` color styles, including `fill`, `stroke`, and text `color`.
- Added: Support for labeled arrows and dotted arrows in Mermaid flowcharts.
- Changed: Kept Mermaid rendering self-contained so `md-pew.html` still works offline without CDN or npm dependencies.
- Verified: Checked JavaScript syntax and rendered the reported Mermaid sample into SVG with the expected class colors.

## 0.1.0 - 2026-04-30

### 中文

- 新增：创建 md-pew 项目。
- 新增：加入第一版独立 Markdown 编辑器和预览器。
- 新增：支持拖拽打开、实时预览、保存/下载和 HTML 导出。
- 新增：加入项目文档，方便长期跟踪。

### English

- Added: Created the md-pew project.
- Added: Added the first standalone Markdown editor and previewer.
- Added: Added drag-and-drop opening, live preview, save/download, and HTML export.
- Added: Added project docs for long-term tracking.
