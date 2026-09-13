# Math Fighter Promotional Video Bootstrap

## Project role

Create a standalone promotional video for **Math Fighter** based on the current development-repository gameplay.

Source project: `fiverocks-dev/math-fighter`

## 1. Game as the player experiences it

### Player-facing game definition

Math Fighter is a math-action shooting game in which the player solves an arithmetic problem, finds the enemy carrying the correct answer, and shoots that target while enemies descend toward the player.

The basic player loop is:

`see problem -> calculate -> find the correct answer-bearing enemy -> shoot -> survive -> next problem`

Current observed gameplay structure:

- A math question is active during battle.
- Multiple enemies descend while displaying different answer values.
- One enemy corresponds to the correct answer.
- The player attacks enemies directly.
- Destroying the correct target resolves the current quiz/wave and advances play.
- Correct and incorrect targets have different score consequences.
- The battle has player health, game-over state, stage-clear flow, and Normal/Challenge stage modes.
- Challenge play advances through levels and tracks best score by arithmetic operation.

### What should be obvious to a new player

Within a few seconds, the viewer should understand:

1. this is a shooting/action game,
2. enemies carry possible answers,
3. the player must calculate before deciding whom to shoot,
4. enemies are moving, so the decision happens under pressure.

This section defines **what the player actually does**.

## 2. Product / design intent

The design connects arithmetic directly to target selection instead of separating quiz solving from combat.

Important design characteristics include:

- the math problem determines which enemy should be attacked,
- the answer is embedded in the combat space rather than presented as a detached multiple-choice screen,
- time pressure comes from descending enemies and player survival,
- incorrect targeting has immediate combat/score consequences,
- Challenge mode extends the same interaction into continuing level progression.

The key design goal is not merely “make math exciting,” but to make calculation a functional part of moment-to-moment action.

## 3. Promotional strategy

### Current promotional hook

Working hook:

**Find the answer. Hit the target.**

Alternative Korean framing:

**정답을 찾아, 격추하라.**

The strongest visual chain is:

`question -> calculate -> identify target -> fire -> target destroyed`

### Campaign experience to communicate

Priority order:

1. Make the viewer understand that answer values are attached to enemies.
2. Show that the player personally selects and shoots the correct target.
3. Then increase speed and combat pressure.
4. Use incorrect-target or health consequences as escalation, not as the opening explanation.

## Hero footage

Priority capture moments:

1. A readable arithmetic question with three answer-bearing enemies descending.
2. A short hesitation/read moment so the viewer can solve with the player.
3. Player firing at the correct answer-bearing enemy.
4. Correct target destruction and wave resolution.
5. Fast follow-up problem showing repeated combat rhythm.
6. Optional contrast: attack an incorrect target and show the consequence.
7. Optional Challenge-stage sequence showing sustained pressure.

## Creative rhythm

Recommended standalone video rhythm:

`SEE THE PROBLEM -> FIND THE TARGET -> FIRE -> CLEAR -> REPEAT -> PRESSURE BUILDS`

Do not cut directly from question to explosion; preserve the targeting decision.

## Visual identity hypothesis

- Fast, arcade-like pacing.
- Strong projectile/hit/explosion sound design.
- Numbers on enemies must remain legible.
- Avoid covering answer values with oversized captions.
- Use screen-space typography mainly between action beats.

## Claims to avoid without re-verification

Do not claim:

- that answering a quiz button automatically causes an attack,
- specific curriculum alignment or learning outcomes,
- specific final release/store status unless verified at production time,
- unsupported progression or upgrade systems.

## Candidate taglines

Game-explaining options:

- **Find the answer. Hit the target.**
- **The answer is one of them. Shoot the right one.**
- **정답을 찾아, 격추하라.**

Action/escalation options:

- **Think fast. Shoot right.**
- **The answer is coming at you.**

These are working creative options, not approved final copy.

## Recommended first deliverable

Create a 20-30 second standalone synopsis/storyboard that first explains one complete readable combat interaction, then escalates into faster waves or Challenge footage.

## Re-verification before production

Before final capture, re-check:

- current `AGENTS.md` and gameplay/status documents in `fiverocks-dev/math-fighter`,
- `StageManager`, enemy/target behavior, stage rules, and relevant tests,
- current playable Android/build status,
- exact UI and score behavior in the build being filmed.
