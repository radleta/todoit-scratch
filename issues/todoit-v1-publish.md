---
tool: write_issue
kind: issue
title: "Publish todoit v1 to GitHub Pages from main"
slug: todoit-v1-publish
status: open
captured: 2026-10-18T18:19:41.803Z
repo: todoit
branch: develop
commit: 92ccd1e
working_tree: 1 modified, 1 untracked
blocked_by: todoit-v1-app
epic: todoit-v1
---
# Issue: Publish todoit v1 to GitHub Pages from main

## Summary
Take todoit v1 live: merge `develop` into `main`, turn on GitHub Pages for `radleta/todoit` publishing from `main`, and confirm the app works at the public Pages URL, todos surviving a reload there. Waits on `todoit-v1-app` landing on `develop` with its Playwright flows passing.

## Context

### Intent
Filed by the todoit-v1 discovery breakdown gate as the second build. It is split from the app because it lands on a different branch and deploy target and must follow the app (merge gate). The user left its design lens to `/brainstorming`.

### Observed State (captured 2026-10-18T18:19:41.803Z)
- **Working directory:** D:\dev\github\todoit
- **Repo / branch:** todoit / develop
- **HEAD:** 92ccd1e — docs: add todoit-expert wiki
- **Working tree:** 1 modified, 1 untracked
- **Recent commits (last 3):**
  - 92ccd1e docs: add todoit-expert wiki
  - cb7c2c9 docs: switch lanes to worktree mode
  - 708441b docs: add CLAUDE.md with lane settings

### Prior Investigation
_Not captured._

## Impact
_Not captured._

## Related
issue: todoit-v1 (epic), issue: todoit-v1-app

## Notes
_Not captured._
