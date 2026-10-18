---
tool: write_issue
kind: issue
title: "Build the todoit v1 app: jar-ring bubbles, IndexedDB storage, tests"
slug: todoit-v1-app
status: open
captured: 2026-10-18T18:19:38.949Z
repo: todoit
branch: develop
commit: 92ccd1e
working_tree: 1 modified, 1 untracked
epic: todoit-v1
lens: long-term investment
---
# Issue: Build the todoit v1 app: jar-ring bubbles, IndexedDB storage, tests

## Summary
Build todoit v1 as a static app of plain HTML and JavaScript modules in the washday look with the jar-ring interaction: add, list, pop to complete, edit, delete and filter todos; restore from done and undo a delete; live counts and an all-time tally; pop sound and effects with a remembered mute toggle and reduced-motion support; todos kept in IndexedDB so they survive a reload and a browser restart. The logic has unit tests that run without a browser, and Playwright tests cover add, pop, filter and reload-keeps-todos. Done when those flows pass on `develop`, which is the bar for going live.

## Context

### Intent
Filed by the todoit-v1 discovery breakdown gate as the first of two builds. The user approved one build for the whole app (no forcing condition splits it) and drafting its design on long-term investment: clean seams between logic, storage, view and effects, so the tests have a place and the later day-jars idea can reuse the storage format.

### Observed State (captured 2026-10-18T18:19:38.949Z)
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
issue: todoit-v1 (epic, ## Decisions), issue: bubble-interaction-prototype, issue: visual-aesthetic-mockups, issue: fun-principles, scratch/E-todoit-v1/prototypes/iteration-2/jar-ring.html, scratch/E-todoit-v1/mockups/washday.html, .claude/skills/todoit-expert/fun-principles.md

## Notes
_Not captured._
