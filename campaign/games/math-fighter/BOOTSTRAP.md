# Math Fighter Promotional Video Bootstrap

## Project role

Create a standalone promotional video for **Math Fighter** based on the current development-repository gameplay.

Source project: `fiverocks-dev/math-fighter`

## 1. Game as the player experiences it

### Player-facing game definition

Math Fighter is a math-action shooting game in which the player solves an arithmetic problem, identifies the enemy carrying the correct answer, moves into that target's zone, and attacks while enemies descend toward the player.

For the current Three-Zone control mode, the player taps one of three horizontal screen zones. The ship moves toward that zone and fires while positioned in the selected zone during active play.

The basic player loop is:

`see problem -> calculate -> find the correct answer-bearing enemy -> choose its zone -> move/fire -> survive -> next problem`

Current observed gameplay structure:

- A math question is active during battle.
- Three enemies descend while displaying different answer values.
- One enemy corresponds to the correct answer.
- The player controls combat positioning and firing behavior; in Three-Zone mode, tapping a zone moves the ship there and enables firing once the ship is inside that zone.
- Destroying the correct target resolves the current quiz/wave and advances play.
- Correct and incorrect targets have different score consequences.
- The battle has player health, game-over state, stage-clear flow, and Normal/Challenge stage modes.
- Challenge play advances through levels and tracks best score by arithmetic operation.

### What should be obvious to a new player

Within a few seconds, the viewer should understand:

1. this is a shooting/action game,
2. enemies carry possible answers,
3. the player must calculate before deciding where to move and attack,
4. enemies are moving, so the decision happens under pressure.

This section defines **what the player actually does**.

## 2. Product / design intent

The design connects arithmetic directly to combat positioning and target selection instead of separating quiz solving from combat.

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

The strongest visual chain for Three-Zone footage is:

`question -> calculate -> identify answer lane -> tap zone -> ship moves/fires -> target destroyed`

### Campaign experience to communicate

Priority order:

1. Make the viewer understand that answer values are attached to enemies.
2. Show that the calculation changes the player's combat-position choice.
3. Show the ship move and fire at the correct target.
4. Then increase speed and combat pressure.
5. Use incorrect-target or health consequences as escalation, not as the opening explanation.

## Hero footage

Priority capture moments:

1. A readable arithmetic question with three answer-bearing enemies descending.
2. A short hesitation/read moment so the viewer can solve with the player.
3. A visible zone choice where the ship is initially away from the correct target.
4. Ship movement into the correct lane followed by firing.
5. Correct target destruction and wave resolution.
6. Fast follow-up problem showing repeated combat rhythm.
7. Optional contrast: attack an incorrect target and show the consequence.
8. Optional Challenge-stage sequence showing sustained pressure.

## Creative rhythm

Recommended standalone video rhythm:

`SEE THE PROBLEM -> FIND THE TARGET -> CHOOSE THE ZONE -> MOVE/FIRE -> CLEAR -> REPEAT -> PRESSURE BUILDS`

Do not cut directly from question to explosion; preserve the player's combat decision.

## Visual identity hypothesis

- Fast, arcade-like pacing.
- Strong projectile/hit/explosion sound design.
- Numbers on enemies must remain legible.
- Avoid covering answer values with oversized captions.
- Use screen-space typography mainly between action beats.
- If raw capture does not reveal the touch itself, prefer a restrained post-production touch indicator rather than fake runtime UI.

## Claims to avoid without re-verification

Do not claim:

- that tapping the enemy itself is the current Three-Zone control mechanic,
- that answering a quiz button automatically causes an attack,
- specific curriculum alignment or learning outcomes,
- specific final release/store status unless verified at production time,
- unsupported progression or upgrade systems.

## Candidate taglines

Game-explaining options:

- **Find the answer. Hit the target.**
- **The answer is one of them. Move. Fire.**
- **정답을 찾아, 격추하라.**

Action/escalation options:

- **Think fast. Shoot right.**
- **The answer is coming at you.**

These are working creative options, not approved final copy.

## Pilot deliverables

The current pilot planning set is:

- `SYNOPSIS.md` — product truth, narrative premise, creative proposition, pilot learning questions
- `STORYBOARD.md` — working 20–25 second vertical-first master structure
- `SHOT_LIST.md` — exact gameplay capture requirements and provenance checklist

The next phase after these documents is real capture and edit testing, followed by 15-second / 6-second cutdowns and a postmortem.

## Current status boundary

The development repository currently tracks a **First Playable Release** epic and remaining first-play/on-device QA and polish work. Treat Math Fighter as a current playable development product, not as a formally released store product unless release evidence is separately verified at delivery time.

At the time of this update, open work includes first-play onboarding, combat-answer feedback polish, progression/difficulty review, Android smoke/QA, and a movement-jitter fix PR. These can materially affect how polished capture footage looks even when they do not change the core concept.

## Re-verification before production

Before final capture, re-check:

- current `AGENTS.md` and gameplay/status documents in `fiverocks-dev/math-fighter`,
- current `main` and all gameplay-relevant open PRs,
- `StageManager`, enemy/target behavior, stage rules, and relevant tests,
- `Player.cs` firing behavior,
- the selected movement/control implementation, especially `ThreeZoneMovementController.cs` if used as the hero mode,
- current playable Android/build status,
- exact UI and score behavior in the build being filmed.
