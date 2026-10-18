---
source: brainstorming/research
type: research
scope: project
target-domain: todoit-expert
target-page: fun-principles
status: captured
---

## What "fun" means in todoit: the five principles from the fun.md transcript

The todoit-v1 epic defines "fun" as the principles in the transcript at `scratch/repo-setup/fun.md`, a game-design video about making a button fun to press. Those principles are the test for every interaction design choice in the app. The transcript calls its model "over simplified" but "close enough that we can do something useful with it". Its principles, in its own order:

| # | Principle | What the transcript means by it |
|---|---|---|
| 1 | **Impact** | Changing your environment gives "a feeling of control and power". Destruction is fun because it gives "a lot of impact quickly and without a lot of effort". Having no impact "feels like a waste of time". More impact is better, so "anything that adds additional impact to your actions is usually a good thing" (its example is knock-back when firing). Permanence matters: "lasting consequences are more fun". The biggest impact is on other people, triggering "thoughts emotions and reactions". |
| 2 | **Reward** | The "chocolate" for an action, with "acoustic rewards and eye candy" as the obvious ones: sounds, particles, wobble, shaking, haptic rumble. Reward and impact are "very closely related". "Lasting rewards tend to feel more valuable" (the XP bar that levels you up). "Artificially delaying them a bit" makes rewards more desirable (loot-box opening animations). Randomness does too, though the transcript calls randomized XP "an abusive gambling game" and "morally questionable". |
| 3 | **Challenge** | "Too much of it feels stressful and frustrating, too little of it feels boring", so keep people between the two. "Attaching rewards to challenges is a sensible thing to do". A good challenge "should also feel fair and provide you with plenty of feedback on how well you're doing". |
| 4 | **Fantasy** | People like empathizing, stories, and escaping reality. Framing alone changes the feel "even though the gameplay is completely the same": the same button becomes "the master button in the fun spaceship". |
| 5 | **People differ** | This applies to all three categories (challenge, reward, fantasy): "different people want different challenges different rewards different fantasies". There are "no one-size-fits-all solutions", and "if somebody doesn't like space you might even be better off keeping it abstract". |

### What each principle requires of a todoit interaction

| Principle | Rule for todoit interactions |
|---|---|
| Impact | Every action (add, pop, edit, delete, filter) visibly moves the bubble field right away, at the cost of one gesture. The empty state has something to press, because a screen with nothing to affect is the "waste of time" case. Completion leaves a lasting trace: a popped todo lives on under the done filter, so a pop never looks undone or lost. |
| Reward | Popping a bubble gets the strongest sound and eye candy in the app. Any delay before the reward lands is a short animation; the todo's state change is never held back. Randomness stays cosmetic (pitch, particle colour, spread) and never varies what an action earns. |
| Challenge | The challenge is the visitor's own tasks, not the controls, so a pop never needs aim or timing. Reward goes where the challenge is: completing gets more than adding, and deleting gets less than completing so that discarding a task never feels like finishing it. The fair-feedback rule means the visitor can always see how they are doing, for example how many todos are active and how many are done. |
| Fantasy | Bubbles are a frame, and the look (water, sky, space, or none) is chosen as a fantasy. An abstract look is an acceptable choice. Wording and the empty state stay inside the chosen frame. |
| People differ | No effect is forced on anyone: sound can be turned off, and motion respects the system's reduced-motion setting. A theme never gets in the way of plain use. |

### Where the principles pull against each other

- **Challenge against impact:** impact wants big effects "quickly and without a lot of effort", while challenge wants difficulty. In a todo app the controls stay effortless and the difficulty comes from the tasks.
- **Reward randomness against the transcript's own caveat:** randomness makes rewards more exciting, but the transcript calls it a gambling mechanic, so it stays cosmetic.
- **Fantasy against people differ:** a strong theme loses visitors who dislike it, and the transcript names abstract as the safe fallback.

**Source:** the transcript at [`scratch/repo-setup/fun.md`](../../../scratch/repo-setup/fun.md); the epic decision that adopts it at [`scratch/issues/todoit-v1.md` `"Fun" means`](../../../scratch/issues/todoit-v1.md)
**Discovered:** research spike `fun-principles` (epic `todoit-v1`), 2026-10-18
**Impact:** Anyone designing or changing a todoit interaction after v1, such as a new gesture, a bubble effect, the empty state or a later feature, opens this page to test the change against the project's definition of fun. Without it they would judge "fun" by their own taste or reread a 7-minute transcript.
