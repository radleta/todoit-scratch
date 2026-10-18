---
source: implementation/ad-hoc
type: gotcha
scope: project
target-domain: todoit-expert
target-page: worktree-lanes
status: ingested
ingested-at: 2026-10-18T17:03:08.713Z
---

## lane remove fails on Windows; remove lane worktrees by hand

On Windows, `lane remove {slug}` stops with `<path> is not a worktree of this repo` (exit 2) even for a worktree `lane open` made, and re-running `lane open {slug}` for an existing worktree stops with `exists but is not a worktree of this repo`. The script compares a backslash path against git's forward-slash `worktree list` output. Creating a new lane worktree works.

After `/end-lane`, remove the worktrees from the main checkout with:

    git -C scratch worktree remove ../todoit-{slug}/scratch
    git worktree remove ../todoit-{slug}

To resume a lane whose session was closed, `cd ../todoit-{slug}` and start `claude` there.

**Source:** observed 2026-10-18 with `lane open smoke-test --no-launch` then `lane remove smoke-test`; upstream issue `lane-remove-and-lane-open-reuse-fail-on` in claude-code-ref's `scratch/issues/`
**Discovered:** smoke-testing worktree lanes during repo setup
**Impact:** whoever finishes or resumes a lane on Windows hits this error at cleanup or relaunch and needs the manual commands.
