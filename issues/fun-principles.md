---
tool: write_issue
kind: idea
title: "Fun principles: what the fun.md transcript says makes an interaction fun"
slug: fun-principles
status: settled
captured: 2026-10-18T17:27:16.151Z
repo: todoit
branch: develop
commit: 92ccd1e
working_tree: clean
role: spike
epic: todoit-v1
spike_type: research
---
# Idea: Fun principles: what the fun.md transcript says makes an interaction fun

## Summary
Extract the principles in `scratch/repo-setup/fun.md` (a YouTube transcript on making a button fun to press) and state what each one implies for todoit: adding, popping to complete, editing, deleting and filtering todo bubbles. The principles become the epic's definition of fun and are captured for the todoit-expert wiki.

## Context

### Intent
_Not captured._

### Observed State (captured 2026-10-18T17:27:16.151Z)
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
scratch/repo-setup/fun.md

## Notes
_Not captured._

## Resolution (2026-10-18)

Fun in todoit means the transcript's five principles, applied in its order: impact, reward, challenge, fantasy and people differ, not a looser sense of "playful", because the user set `scratch/repo-setup/fun.md` as the definition of fun for this epic.

Evidence, from the `researcher` reading of `scratch/repo-setup/fun.md` (captured for the wiki at `scratch/todoit-v1/learned/research-fun-principles.md`):

- **Impact.** Actions change the surroundings "quickly and without a lot of effort"; "lasting consequences are more fun". For todoit: a new todo arrives with force (the transcript's own example is "holding the button creates a bubble and releasing it shoots it away"), popping is the big one-gesture destruction moment, and the done view is where a pop leaves its lasting mark. The empty state must give the visitor something to press.
- **Reward.** "Acoustic rewards and eye candy"; lasting rewards feel more valuable; a short delay builds anticipation; randomness excites but the transcript calls randomized rewards "morally questionable". For todoit: popping gets the strongest sound and visuals, a short animation may delay the reward but never the state change, and randomness stays cosmetic (pitch, particle colour), never in what an action earns.
- **Challenge.** Between stress and boredom, fair, with "plenty of feedback on how well you're doing"; attach rewards to challenges. For todoit: the challenge is the visitor's own tasks, never the controls (a pop needs no aim or timing); completing earns more than adding, deleting earns less than completing; active and done counts are always visible.
- **Fantasy.** Framing alone changes how the same action feels. For todoit: bubbles are a light fantasy, and each look-and-feel mockup is in effect a choice of fantasy, with abstract a legitimate option.
- **People differ.** "No one-size-fits-all solutions". For todoit: sound can be muted, motion respects the reduced-motion setting, and no theme blocks plain use.

Tensions the researcher named against the epic: a popped bubble must still show in the done filter; permanence pulls against undoing an accidental pop or delete; an XP-style counter would exceed v1 scope, where a plain count does not; impact on other people is out of reach with local-only storage; and effects cannot be checked by the DOM-free unit tests.
