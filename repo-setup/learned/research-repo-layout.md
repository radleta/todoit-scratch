---
source: implementation/ad-hoc
type: research
scope: project
target-domain: todoit-expert
target-page: repo-layout
status: ingested
ingested-at: 2026-10-18T17:03:07.888Z
---

## todoit is two git repos: code and a nested scratch repo

The checkout holds two independent git repos. The code repo (`radleta/todoit` on GitHub, public) is the checkout root; its `.gitignore` excludes `scratch/`. The scratch repo (`radleta/todoit-scratch`, public) lives at `scratch/` and holds planning, issues, session handoffs, lane records and `learned/` captures.

The two repos use different base branches. Code work lands on `develop`, which is the GitHub default branch and the lane baseline set by the `CLAUDE.md` lane line. Scratch work lands on scratch `main`. The code repo's `main` stays at the initial commit; nothing in the lane workflow moves it, so promoting `develop` to `main` is a manual step.

Every git command for scratch runs as `git -C scratch ...`; a plain `git` command at the root never sees scratch files.

**Source:** [`CLAUDE.md` `Lanes`](../../../CLAUDE.md), [`.gitignore` `scratch/`](../../../.gitignore)
**Discovered:** initial repo setup, 2026-10-18
**Impact:** anyone opening a PR, cutting a release or committing planning docs needs to know which repo and which branch a change belongs on; without this they target `main` or commit scratch files from the root and see nothing staged.
