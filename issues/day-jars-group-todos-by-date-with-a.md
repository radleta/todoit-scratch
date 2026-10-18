---
tool: write_issue
kind: idea
title: "Day jars: group todos by date with a shelf of jars for the coming days"
slug: day-jars-group-todos-by-date-with-a
status: open
captured: 2026-10-18T18:17:03.119Z
repo: todoit
branch: develop
commit: 92ccd1e
working_tree: 1 modified, 1 untracked
---
# Idea: Day jars: group todos by date with a shelf of jars for the coming days

## Summary
Group todos by date and show a shelf of jars, one per day for the next several days, so the visitor sees at a glance how much is planned for each day. Each jar shows a placeholder for every undone todo and a solid marble for every done one. The shelf doubles as a way to organize and filter todos by day.

## Context

### Intent
Came out of the todoit-v1 discovery's second prototype round. The user picked `jar-ring` for v1 but said of `jar-shelf`: "I really like the way the shelf provides a way to organize and filter that direction. So that a way for us to group things by date. But then the next seven days shows as different jars that shows you kind of how much to do things." Kept outside the todoit-v1 epic on purpose: "that's the direction we need, but not inside this epic as I want to try to push towards a release."

### Observed State (captured 2026-10-18T18:17:03.119Z)
- **Working directory:** D:\dev\github\todoit
- **Repo / branch:** todoit / develop
- **HEAD:** 92ccd1e — docs: add todoit-expert wiki
- **Working tree:** 1 modified, 1 untracked
- **Recent commits (last 3):**
  - 92ccd1e docs: add todoit-expert wiki
  - cb7c2c9 docs: switch lanes to worktree mode
  - 708441b docs: add CLAUDE.md with lane settings

### Prior Investigation
The user's direction: "the jars should show kind of like we did, like in a way where you can see like the next couple of days. The jars should show placeholders for undone things and then it should show solid for done." The user expects "a lot of little tweaks and twists and turns" and that it will need new mockups and prototypes to feel out before any design. The round-2 prototype `jar-shelf.html` is the starting point: today's jar with one dashed slot per todo, and a shelf of past days' jars marked "n of m". It shows past days only, its history is sample data, and the move of a day's jar onto the shelf is described but not built. Open questions it raises include how a todo gets its date, what happens to an undone todo when its day passes, and how the day filter sits beside all/active/done.

## Impact
_Not captured._

## Related
scratch/E-todoit-v1/prototypes/iteration-2/jar-shelf.html, scratch/E-todoit-v1/prototypes/iteration-2/jar-shelf-desktop.png, issue: todoit-v1 (Out of Scope), issue: bubble-interaction-prototype

## Notes
_Not captured._
