# Math Rain Promotional Video Bootstrap

## Project role

Create a standalone promotional video for **Math Rain** that sells the real-time pressure, combo rhythm, and visible consequence of answer choices.

Source project: `fiverocks-dev/math-rain`

## Evidence-grounded game definition

Math Rain is a browser-based real-time math arcade game.

Current implementation behavior:

- Math problems appear as falling raindrops.
- The player chooses from answer cards.
- Correct selection resolves the matching problem.
- Correct answers increase score and combo.
- Incorrect selection resets combo and pushes every unresolved raindrop farther downward.
- A raindrop reaching the danger line costs one life.
- The player begins with three lives.
- Difficulty changes falling speed.
- Supported operations include addition, subtraction, multiplication, division, and mixed modes.
- A level is divided into multiple stages, with problem volume scaling by level.
- Current code contains a one-time revive path under the appropriate game-over condition.

The important distinction is that a wrong answer does not merely reduce a score value; it makes the live board more dangerous.

## Core promotional hook

**Every wrong answer brings the problem closer.**

Alternative Korean framing:

**틀리면, 문제가 더 가까워진다.**

The strongest visual chain is:

`falling problem -> calculate -> choose card -> threat disappears OR the whole board drops closer`

## Audience experience to communicate

The viewer should understand that:

1. this is played under real-time pressure,
2. one answer can change the state of the whole board,
3. accuracy and speed feed a combo rhythm,
4. survival matters, not just quiz completion.

## Hero footage

Priority capture moments:

1. Several readable problems falling simultaneously.
2. Answer-card row visible beneath them.
3. Correct answer selection clearing a problem with score/combo increase.
4. A deliberate wrong-answer capture where unresolved raindrops visibly jump downward.
5. A near-miss moment with a raindrop close to the bottom.
6. A lost-life moment.
7. A short high-combo sequence with fast correct selections.
8. Optional difficulty contrast using clearly different falling speeds.

## Creative rhythm

Recommended standalone video rhythm:

`SEE -> CALCULATE -> TAP -> CLEAR -> COMBO -> PRESSURE RISES`

The edit should accelerate as the board fills. A brief wrong-answer beat can serve as the dramatic midpoint before the player recovers into a combo.

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

- **Solve before they fall.**
- **Think fast. Keep the rain up.**
- **One wrong answer changes everything.**
- **떨어지기 전에 풀어라.**
- **정답은 콤보가 되고, 오답은 위기가 된다.**

These are working creative options, not approved final copy.

## Recommended first deliverable

Create a 20-25 second standalone synopsis/storyboard built around a clean escalation: easy board -> combo -> wrong answer -> danger -> recovery.

## Re-verification before production

Before final capture, re-check:

- current repository README/docs and `src/game.ts`,
- tests for score, combo, lives, wrong-answer movement, stage completion, and revive,
- current public/build state and exact configuration used for capture,
- operation/difficulty options visible in the production build.
