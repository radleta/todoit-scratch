---
session_id: todoit
schema_version: 3
last_pointer_rewrite: 2026-10-18T18:22:24.408Z
session_count: 1
---

## Open questions (still open)

- none

## Goal

This is the product and project management workstream for todoit, a small todo app that illustrates the user's Claude Code skills, agents and commands. It designs and manages the work: discovery, epics, spikes, issues, prototypes, the wiki and grooms. Building happens in separate lane sessions (`lane open {issue-slug}`), where `/brainstorming` and `/implement-code` run. The current destination is the `todoit-v1` epic: a fun, usable todo app live on GitHub Pages.

## Next best step

The user is building `todoit-v1-app` in its own lane (`lane open todoit-v1-app`, worktree `D:/dev/github/todoit-todoit-v1-app`). This workstream waits for that lane to land on `develop`. When it has, run `/close-issue todoit-v1-app` from the main checkout: its epic groom ticks the app's outcomes on `scratch/issues/todoit-v1.md` and re-runs the breakdown gate, which makes `todoit-v1-publish` (`scratch/issues/todoit-v1-publish.md`, blocked by the app) the next workable build. Check `git log --oneline -5 develop` and `git -C scratch log --oneline -5` first to see what the lane landed.

## Latest summary

Set up todoit (public repos, develop baseline, worktree lanes, todoit-expert wiki), ran /discovery on todoit-v1 through fun principles and two prototype rounds, and filed the app and publish builds

## Sessions
| timestamp | summary | file |
|---|---|---|
| 2026-10-18T18:22:24.390Z | Set up todoit (public repos, develop baseline, worktree lanes, todoit-expert wiki), ran /discovery on todoit-v1 through fun principles and two prototype rounds, and filed the app and publish builds | [sessions/2026-10-18T18-22-24-390Z-5a43fdb3.md](sessions/2026-10-18T18-22-24-390Z-5a43fdb3.md) |
