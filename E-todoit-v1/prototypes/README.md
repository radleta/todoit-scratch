# Bubble interaction prototypes

Throwaway prototypes for the `bubble-interaction-prototype` spike. Each one is a single HTML file that opens straight from disk, with no build step and no network requests. State lives in memory and resets on reload. The styling is deliberately plain, because the look gets chosen from the mockups. These files are about feel.

All three share the same base. Type a todo, then hold **Hold to blow**: the bubble grows while you hold and shoots in when you let go (Enter fires a medium shot). Tap a bubble to pop it, which completes it. Sound starts after your first tap and has a mute toggle. You also get All/Active/Done filters with live counts, an all-time popped tally, restore from Done, delete (the × on a bubble or in Done) with a 5-second Undo toast, a "pop me" practice bubble when nothing is left, and a Motion control (follow system, full or reduced). In reduced motion the bubbles sit still in reading order and a pop is a quick fade.

| File | What makes it different | Leans on |
| --- | --- | --- |
| `bubbles-slingshot.html` | Bubbles ricochet with almost no friction. A pop is a loud blast that shoves nearby bubbles and shakes the field, and the popped todo stays as a flattened "splat" in the done shelf. | Impact |
| `bubbles-jar.html` | Bubbles float up like balloons. The count changes the moment you tap, then the bubble tenses for a beat before it bursts, and a marble flies into a jar that keeps every pop. | Reward (anticipation, a lasting record) |
| `bubbles-cluster.html` | Bubbles pack into one cluster inside a progress ring that fills as you pop ("3 of 8 popped"). A pop ripples through its neighbours, and quick pops in a row rise in pitch (cosmetic only). Done shows "pop marks" with a time. | Challenge (feedback on how you're doing) |

People differ is covered the same way in all three: a mute toggle and reduced-motion support. The fantasy is bubbles in every variant.
