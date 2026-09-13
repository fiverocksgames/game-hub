# Math Fighter Promotional Video Bootstrap

## Project role

Create a standalone promotional video for **Math Fighter** based on the current development-repository gameplay, not on generic educational-game positioning.

Source project: `fiverocks-dev/math-fighter`

## Evidence-grounded game definition

Math Fighter is a math-action shooting game in which arithmetic is used to identify the correct combat target.

Current observed gameplay structure:

- A math question is active during battle.
- Multiple enemies descend while displaying different answer values.
- One enemy corresponds to the correct answer.
- The player attacks enemies directly.
- Destroying the correct target resolves the current quiz/wave and advances play.
- Correct and incorrect targets have different score consequences.
- The battle has player health, game-over state, stage-clear flow, and Normal/Challenge stage modes.
- Challenge play advances through levels and tracks best score by arithmetic operation.

The important distinction is that the game is **not** a passive quiz followed by a decorative attack animation. The arithmetic result is used to identify which moving enemy should be attacked.

## Core promotional hook

**Calculate the target. Then fight.**

Alternative Korean framing:

**답을 고르는 게 아니라, 정답을 쏜다.**

The strongest visual idea is the instant connection between:

`question -> calculate -> identify answer-bearing enemy -> shoot -> wave resolves`

## Audience experience to communicate

The viewer should understand within a few seconds that:

1. this is a real action game,
2. arithmetic changes moment-to-moment targeting,
3. speed and accuracy both matter,
4. mistakes have visible gameplay consequences.

## Hero footage

Priority capture moments:

1. A readable arithmetic question with three answer-bearing enemies descending.
2. A short hesitation/read moment so the viewer can solve with the player.
3. Player firing at the correct answer-bearing enemy.
4. Correct target destruction and wave resolution.
5. Optional contrast: attack an incorrect target and show the negative score consequence.
6. Fast Challenge-stage sequence showing increasing level pressure.

## Creative rhythm

Recommended standalone video rhythm:

`SEE THE PROBLEM -> FIND THE TARGET -> FIRE -> SURVIVE -> GO AGAIN`

The edit should preserve enough time before the shot for the audience to understand that a decision was made.

## Visual identity hypothesis

- Fast, arcade-like pacing.
- Strong projectile/hit/explosion sound design.
- Numbers on enemies must remain legible.
- Avoid covering answer values with oversized captions.
- Use screen-space typography only between action beats.

## Claims to avoid without re-verification

Do not claim:

- that answering a quiz button automatically causes an attack,
- specific curriculum alignment or learning outcomes,
- specific final release/store status unless verified at production time,
- unsupported progression or upgrade systems.

## Candidate taglines

- **Find the answer. Hit the target.**
- **Think fast. Shoot right.**
- **The answer is coming at you.**
- **정답을 찾아, 격추하라.**

These are working creative options, not approved final copy.

## Recommended first deliverable

Create a 20-30 second standalone synopsis/storyboard built around one complete readable combat interaction, then expand into rapid escalation and Challenge footage.

## Re-verification before production

Before final capture, re-check:

- current `AGENTS.md` and gameplay/status documents in `fiverocks-dev/math-fighter`,
- `StageManager`, enemy/target behavior, stage rules, and relevant tests,
- current playable Android/build status,
- exact UI and score behavior in the build being filmed.
