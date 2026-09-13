# Math Rain Promotional Video Bootstrap

## Project role

Create a standalone promotional video for **Math Rain** using the current development-repository gameplay as the factual basis.

Source project: `fiverocks-dev/math-rain`

## 1. Game as the player experiences it

### Player-facing game definition

Math Rain is a real-time math arcade game in which math problems fall downward and the player must solve them by selecting the matching answer card before they reach the bottom.

The basic player loop is:

`see a falling problem -> calculate -> choose the matching answer card -> clear the problem -> keep surviving`

Current implementation behavior:

- Math problems appear as falling raindrops.
- The player chooses from answer cards.
- Correct selection resolves the matching problem.
- Correct answers increase score and combo.
- Incorrect selection resets combo and pushes unresolved raindrops farther downward.
- A raindrop reaching the danger line costs one life.
- The player begins with three lives.
- Difficulty changes falling speed.
- Supported operations include addition, subtraction, multiplication, division, and mixed modes.
- A level is divided into multiple stages, with problem volume scaling by level.
- Current code contains a one-time revive path under the appropriate game-over condition.

### What should be obvious to a new player

Within a few seconds, a viewer should be able to understand:

1. problems are falling,
2. the player solves them by selecting answer cards,
3. unresolved problems create time pressure,
4. the goal is to keep clearing problems and survive.

This section describes **what the game is**, not what the campaign should emphasize.

## 2. Product / design intent

The current gameplay design adds pressure and rhythm to otherwise discrete arithmetic decisions.

Important design characteristics include:

- math is performed continuously rather than as a sequence of static quiz screens,
- the board remains live while the player is deciding,
- correct answers build momentum through score and combo,
- mistakes increase immediate board danger instead of being only an abstract score penalty,
- survival pressure encourages both accuracy and response speed.

The wrong-answer board drop is therefore a **tension system**, not the primary definition of the game.

## 3. Promotional strategy

### Current promotional hook

Working hook:

**Solve before they fall.**

Alternative Korean framing:

**떨어지기 전에 풀어라.**

The strongest visual chain for advertising is:

`falling problem -> calculate -> choose card -> problem clears -> more problems arrive`

A wrong-answer moment can be used later in the video to demonstrate escalation:

`wrong choice -> unresolved board drops -> danger increases`

### Campaign experience to communicate

The promotional video should first make the game understandable, then make it exciting.

Priority order:

1. Explain visually that falling math problems are cleared by selecting answer cards.
2. Show the real-time race against the falling board.
3. Show satisfying correct-answer chains and combo rhythm.
4. Use wrong-answer acceleration as a tension beat, not as the game definition.
5. Show survival/life pressure only after the core interaction is clear.

## Hero footage

Priority capture moments:

1. Several readable problems falling simultaneously.
2. Answer-card row visible beneath them.
3. One clear problem -> answer-card interaction that a first-time viewer can follow.
4. Correct selection clearing the matching problem.
5. Short sequence of consecutive correct answers with combo/score growth.
6. A deliberate wrong-answer capture where unresolved raindrops visibly jump downward.
7. A near-miss or lost-life moment after the mechanic has already been established.
8. Optional difficulty contrast using clearly different falling speeds.

## Creative rhythm

Recommended standalone video rhythm:

`SEE -> SOLVE -> TAP -> CLEAR -> REPEAT -> PRESSURE BUILDS`

The video should not open on punishment mechanics. Open by teaching the core interaction through action, then escalate the tension.

## Visual identity hypothesis

- Vertical-friendly composition is naturally strong because threats fall downward.
- Use sound to make correct clears and combo escalation satisfying.
- Wrong-answer sound should be immediately paired with the visible board drop.
- Preserve answer-card legibility; do not bury the actual choice under captions.

## Claims to avoid without re-verification

Do not claim without current verification:

- formal learning outcomes or curriculum coverage,
- exact final release status,
- monetization/revive behavior as a consumer-facing promise,
- unsupported 3-digit behavior merely because a `Digits` type exists; verify the actual implemented generation path before advertising it.

## Candidate taglines

Game-explaining options:

- **Solve before they fall.**
- **Falling problems. Find the answers.**
- **떨어지는 문제를 풀어라.**

Tension/escalation options:

- **Think fast. Keep the rain up.**
- **One wrong answer changes the board.**
- **정답은 콤보가 되고, 오답은 위기가 된다.**

These are working creative options, not approved final copy.

## Recommended first deliverable

Create a 20-25 second standalone synopsis/storyboard with this order:

`core mechanic explanation -> satisfying correct-answer rhythm -> rising pressure -> mistake/danger beat -> recovery or survival payoff`

## Re-verification before production

Before final capture, re-check:

- current repository README/docs and `src/game.ts`,
- tests for score, combo, lives, wrong-answer movement, stage completion, and revive,
- current public/build state and exact configuration used for capture,
- operation/difficulty options visible in the production build.
