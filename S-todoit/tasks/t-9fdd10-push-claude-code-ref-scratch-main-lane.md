---
id: t-9fdd10
title: "Push claude-code-ref scratch main: lane-remove capture and its path fix"
status: blocked
created: 2026-10-18T18:22:01.753Z
updated: 2026-10-18T18:22:01.753Z
blocked_on: "the user's go-ahead: pushing a base branch is the user's"
---
Done when: `git -C 'D:/dev/github/claude-code-ref/scratch' status -sb` shows `main` level with `origin/main`.

Two commits on claude-code-ref's scratch `main` are unpushed: `0897de7e capture: lane-remove-and-lane-open-reuse-fail-on` and `02a99800 fix: correct scratch worktree path in lane-remove workaround`. They file the Windows `lane remove` / `lane open` reuse bug found while setting up todoit's worktree lanes.
