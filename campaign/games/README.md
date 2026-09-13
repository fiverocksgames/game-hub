# Per-Game Campaign Projects

This directory contains independent promotional-video campaign projects for individual FiveRocks Games titles.

These projects are separate from the Game Hub multi-game brand campaign in `campaign/CAMPAIGN.md`.

## Project folders

- `math-fighter/`
- `math-defender/`
- `math-rain/`
- `memory-game/`
- `match-fix/`

Each project begins with `BOOTSTRAP.md`.

## Required separation inside each BOOTSTRAP

Every per-game bootstrap must keep these three perspectives distinct:

1. **Game as the player experiences it**
   - What the player sees and does.
   - Core loop and objective.
   - What a first-time viewer should understand without knowing the design intent.

2. **Product / design intent**
   - What the game is trying to achieve through those mechanics.
   - Why specific systems exist.
   - Tension, strategy, pacing, learning, retention, or other design goals.
   - These are not substitutes for the player-facing game definition.

3. **Promotional strategy**
   - Which part of the real game should lead the video.
   - What hook, escalation, or editing structure best communicates it.
   - A strong promotional hook may emphasize one mechanic, but must not be mistaken for the definition of the whole game.

For example, in Math Rain, wrong answers pushing unresolved problems downward is a tension mechanic. The player-facing game definition is broader: solve falling math problems by selecting matching answer cards before they reach the bottom.

## Working model

Per-game campaign work should normally evolve in this order:

1. `BOOTSTRAP.md` — player-facing game truth, product/design intent, promotional strategy, evidence boundaries
2. `SYNOPSIS.md` — narrative concept and campaign proposition
3. `STORYBOARD.md` — timed visual plan
4. `SHOT_LIST.md` — exact capture requirements and build references
5. `COPY.md` — titles, captions, CTA, ad variants
6. `PRODUCTION_LOG.md` — decisions, evidence, revisions, export notes

Before finalizing footage or claims, re-check the corresponding `fiverocks-dev/<game>` development repository and record the exact playable/build state used for capture.
