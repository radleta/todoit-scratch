# Bubble prototypes, iteration 2: jar plus progress

Three throwaway prototypes, all in the washday look, each building the round-1 cluster ring's progress into the jar in a different way. They share the round-1 jar core: hold to blow, tap to pop (the count changes at once, the bubble shivers, bursts and drops a marble into the jar), sound after your first tap with a mute toggle, All/Floating/Popped filters with live counts, restore ("Blow again") from Popped, delete with a 5-second Undo toast, a "pop me" practice bubble when nothing is left, and a Motion control. Every file opens from disk with no network requests. Each one starts with six todos (two already popped) and 23 on the all-time tally, which the header pill shows in all three.

Counts and the "3 of 8" readout change the moment you pop. The jar's picture (pile, slot or ring) moves only when the marble lands. When the last marble of the list lands, the page plays a fanfare, shows "List cleared!" and bursts marbles out of the jar.

| File | How it shows progress | Leans on |
| --- | --- | --- |
| `jar-fill-line.html` | The jar is the current list. A dashed "full" line near the top marks every todo popped, with one notch per todo. Each marble raises the pile toward the line, and when the list is cleared the lid drops on. | Challenge: you can always see how close you are |
| `jar-shelf.html` | Today's jar has one dashed slot per todo, so it is full exactly when the list is cleared, and then it gets its lid. Underneath, a shelf holds small jars from earlier days, each with its marbles and its "n of m", as a lasting record. | Reward and impact: a record that lasts |
| `jar-ring.html` | The cluster's ring wraps the jar and fills as each marble lands, with "3 of 8" beside it. The ring belongs to this list. The jar holds every pop ever made and never empties, so the two never mix. | Challenge feedback (the ring) next to a lasting reward (the jar) |

Screenshots: `jar-{name}-desktop.png` (1280 wide), `jar-{name}-phone.png` (390 wide) and `jar-{name}-cleared.png` (just after the list is cleared).
