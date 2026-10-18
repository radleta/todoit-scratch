---
tool: write_issue
kind: idea
title: "Visual aesthetic mockups: candidate looks for the user to pick from"
slug: visual-aesthetic-mockups
status: settled
captured: 2026-10-18T17:27:20.729Z
repo: todoit
branch: develop
commit: 92ccd1e
working_tree: clean
role: spike
blocked_by: fun-principles
epic: todoit-v1
spike_type: prototype
---
# Idea: Visual aesthetic mockups: candidate looks for the user to pick from

## Summary
Produce several static mockups of todoit's look (palette, type, bubble style, background, empty state), each a distinct direction shaped by the fun principles, for the user to pick one. The resolution names every mockup file and the one chosen.

## Context

### Intent
_Not captured._

### Observed State (captured 2026-10-18T17:27:20.729Z)
- **Working directory:** D:\dev\github\todoit
- **Repo / branch:** todoit / develop
- **HEAD:** 92ccd1e — docs: add todoit-expert wiki
- **Working tree:** clean
- **Recent commits (last 3):**
  - 92ccd1e docs: add todoit-expert wiki
  - cb7c2c9 docs: switch lanes to worktree mode
  - 708441b docs: add CLAUDE.md with lane settings

### Prior Investigation
_Not captured._

## Impact
_Not captured._

## Related
_Not captured._

## Notes
- 2026-10-18: Bound by `fun-principles`. Each mockup is in effect a choice of fantasy (water, sky, space, and so on), and abstract is a legitimate option for visitors who dislike a theme. The empty state and wording stay inside the chosen theme. Active and done counts stay visible in every mockup, and no theme blocks plain use.
- 2026-10-18: Round 1 feedback from the user: washday is the liked look. Iteration 2 of the interaction prototype is built in it.

## Resolution (2026-10-18)

The look is `washday`: soap bubbles with pastel rims on a pale sky with a sun and green hills, navy text, not the underwater, space or abstract directions, because the user picked it and soap bubbles are what a visitor pops.

Artifacts:
- Chosen: `scratch/E-todoit-v1/mockups/washday.html` (screenshots `washday-desktop.png`, `washday-phone.png`).
- Also offered: `scratch/E-todoit-v1/mockups/tidepool.html`, `orbit.html`, `plain.html`, with screenshots and a README beside them.
- The chosen interaction is built in this look: `scratch/E-todoit-v1/prototypes/iteration-2/jar-ring.html`.

Open from the mockup round: the themed filter names (Floating/Popped) may need the plain word beside them, and the input's hint text is cut off at phone width.
