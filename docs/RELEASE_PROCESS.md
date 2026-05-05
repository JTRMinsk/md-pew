# Release Process / 发布流程

md-pew keeps version history in `CHANGELOG.md`.

md-pew 的版本历史统一记录在 `CHANGELOG.md`。

## Required For Each Iteration / 每次迭代要求

- Add a new `CHANGELOG.md` entry before finishing the iteration.
- Use the format `x.y.z - YYYY-MM-DD`.
- Write each entry in Chinese first, then English.
- Keep `README.md` and `CHANGELOG.md` bilingual.
- Record user-facing changes, important implementation notes, and verification.
- Mention limitations when a feature is intentionally partial.

- 每次迭代结束前，都要在 `CHANGELOG.md` 新增记录。
- 使用 `x.y.z - YYYY-MM-DD` 格式。
- 每条记录先写中文，再写英文。
- `README.md` 和 `CHANGELOG.md` 都保持中英双语。
- 记录用户可见改动、重要实现说明和验证结果。
- 如果某个功能是刻意做成部分支持，要明确写出限制。

## Versioning / 版本号规则

- Patch version: fixes, small improvements, docs, or narrowly scoped rendering support.
- Minor version: new user-facing workflows or larger Markdown/preview features.
- Major version: breaking file behavior, packaging model, or data compatibility changes.

- Patch version：修复、小改进、文档更新，或范围较窄的渲染支持。
- Minor version：新的用户工作流，或较大的 Markdown/预览功能。
- Major version：破坏文件行为、打包方式或数据兼容性的变更。

## Current Source Of Truth / 当前唯一来源

The latest released version is the topmost version entry in `CHANGELOG.md`.

最新发布版本以 `CHANGELOG.md` 最上方的版本条目为准。
