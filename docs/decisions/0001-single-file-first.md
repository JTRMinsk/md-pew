# Decision 0001: Start With a Single Local HTML App

Date: 2026-04-30

## Context

md-pew should be easy to use on both Windows and macOS. The first target is a file the user can double-click, then drag a Markdown file into for editing and previewing.

The local environment currently has Node.js but does not have Rust/Cargo, so a Tauri build cannot be produced here yet.

## Decision

Start with a self-contained `md-pew.html` application with no build step and no external runtime dependencies.

## Consequences

- The app is immediately usable and easy to share.
- Browser file-write behavior depends on the browser. Chrome and Edge can usually save back to a picked file; other browsers may require downloading a copy.
- The code should stay structured so it can later be moved into a Tauri/TypeScript app without rewriting the UX from scratch.
