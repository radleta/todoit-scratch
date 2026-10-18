---
tool: write_issue
kind: idea
title: "Bubble interaction prototype: todos as bubbles you pop to complete"
slug: bubble-interaction-prototype
status: settled
captured: 2026-10-18T17:27:18.478Z
repo: todoit
branch: develop
commit: 92ccd1e
working_tree: clean
role: spike
blocked_by: fun-principles
epic: todoit-v1
spike_type: prototype
---
# Idea: Bubble interaction prototype: todos as bubbles you pop to complete

## Summary
Build a rough, throwaway interactive prototype where todos float as bubbles and popping one completes it, applying the fun principles, so the user can react to how it feels before any build designs it. The resolution names the prototype file(s) and the interaction the user picks.

## Context

### Intent
_Not captured._

### Observed State (captured 2026-10-18T17:27:18.478Z)
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
- 2026-10-18: Bound by `fun-principles`. The pop is the app's big one-gesture destruction moment and gets the strongest sound and visuals; it never needs aim or timing. A new todo arrives with force (the transcript's "holding the button creates a bubble and releasing it shoots it away"). A short pop animation may delay the reward but never the state change. Randomness stays cosmetic. Sound can be muted and motion respects reduced-motion. The prototype has to show what a popped todo looks like in the done filter, which is where a pop leaves its lasting mark.
- 2026-10-18: Round 1 feedback from the user: the jar concept (`bubbles-jar.html`) feels best, "where you can see the little jars filling up"; the cluster variant's progress ring also feels good. Asked for a second iteration that translates the progress ring into the jar concept, in the washday look.

## Resolution (2026-10-18)

The bubble interaction is `jar-ring`: tap a bubble to pop it, a marble drops into a jar that keeps every pop ever, and a progress ring around the jar fills for the current list, not the slingshot blast or the packed cluster and not the fill-line or shelf jars, because the user picked it after two rounds as the jar they liked with the cluster's ring turned into it.

Artifacts:
- Chosen: `scratch/E-todoit-v1/prototypes/iteration-2/jar-ring.html` (screenshots `jar-ring-desktop.png`, `jar-ring-phone.png`, `jar-ring-cleared.png` beside it).
- Round 1: `scratch/E-todoit-v1/prototypes/bubbles-slingshot.html`, `bubbles-jar.html`, `bubbles-cluster.html` (README beside them). User feedback: the jar felt best ("you can see the little jars filling up"), and the cluster's progress ring also felt good.
- Round 2, all in the washday look: `scratch/E-todoit-v1/prototypes/iteration-2/jar-fill-line.html`, `jar-shelf.html`, `jar-ring.html` (README beside them).

What the chosen prototype does, as evidence for the design: hold "Hold to blow" to grow a bubble and release to launch it; a tap pops a bubble and its counts change at once, with only the marble animating; sound starts after the first tap with a mute toggle; all/active/done filters with live counts; the jar carries a "N since you started" label as the all-time tally and keeps a restored todo's marble; the ring shows "x of y popped" for the current list; clearing the list plays a fanfare, shows "List cleared!" and turns the ring gold; restore from done; delete with a 5-second undo toast; a "pop me" practice bubble when empty; reduced motion supported. Checked by a scripted Chrome walk with no console errors; sound and feel have not been tried by a person, and bubbles crowd the top of the field.

The shelf variant's grouping by date went to a separate idea outside this epic, `day-jars-group-todos-by-date-with-a`.
