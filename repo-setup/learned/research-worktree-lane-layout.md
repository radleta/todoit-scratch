---
source: implementation/ad-hoc
type: research
scope: project
target-domain: todoit-expert
target-page: worktree-lanes
status: ingested
ingested-at: 2026-10-18T17:03:08.291Z
---

## A worktree lane is a sibling folder with its own scratch worktree

`lane open {slug}`, run from the main checkout, creates a code worktree at `../todoit-{slug}` (a sibling of the main checkout, e.g. `D:/dev/github/todoit-{slug}`) detached at the main checkout's current `HEAD`, and inside it a worktree of the scratch repo at `scratch/`, detached at scratch `main`. It then starts `claude` in that folder with `/begin-lane {slug}`, which moves both worktrees onto `lane/{slug}`. `--no-launch` makes the worktrees without starting `claude`.

Because the code worktree forks from the main checkout's `HEAD`, the main checkout should be on `develop` when a lane is opened. `lane open` also sets `receive.denyCurrentBranch updateInstead` in both repos, which is what lets `/end-lane` land into the checkout that has the base checked out.

Work that builds starts with `lane open`, never inside the main checkout.

**Source:** [`CLAUDE.md` `Lanes`](../../../CLAUDE.md); observed by running `lane open smoke-test --no-launch`, 2026-10-18
**Discovered:** smoke-testing worktree lanes during repo setup
**Impact:** whoever starts a feature needs the launch command and must know the new folder is a sibling, not a subfolder; whoever opens a lane while the main checkout sits on another branch gets a lane forked from the wrong base.
