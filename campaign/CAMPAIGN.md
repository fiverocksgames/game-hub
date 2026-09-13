# Game Hub Google Ads Campaign Brief

## Status

- Campaign: Google Ads brand video for FiveRocks Games Game Hub
- Working branch: `campaign/google-ads-brand-video`
- Document role: canonical campaign brief
- Creative status: concept and 30-second direction established; capture planning and production details remain in progress

## Objective

Promote FiveRocks Games Game Hub by showing the actual character of FiveRocks gameplay rather than presenting Game Hub as a generic collection of educational games.

The campaign should make viewers understand that FiveRocks games repeatedly turn thinking into an immediate gameplay decision and visible consequence.

The video is not a catalog reel whose primary purpose is to enumerate titles. It is a brand-oriented gameplay film that uses multiple games to reveal a shared design idea.

## Audience-facing proposition

Working creative proposition:

**THINK. CHOOSE. ACT.**

Supporting interpretation:

> Knowing the answer is only the beginning.

The player is not rewarded merely for possessing an answer. The player must use judgment in a game action: identify a target, choose under pressure, remember a location, spend earned resources strategically, or physically transform a puzzle state.

## Brand relationship

The campaign should close with the existing FiveRocks Games brand line:

**Play. Think. Grow.**

`THINK. CHOOSE. ACT.` is a campaign editing and messaging device, not a replacement for the company brand line.

## Core creative structure

Across different games, edit toward the same perceptual chain:

`understand -> decide -> act -> visible consequence`

The viewer should be able to see the decision being made. Avoid cutting directly from question to success animation if doing so hides the gameplay choice.

The creative value comes from repeating this structure across different genres.

## Current game evidence and campaign role

The descriptions below are based on development-repository evidence, not public-homepage marketing summaries. Before final capture, re-verify each game's current development repository because implementation status may change.

### Math Fighter

Campaign role: fast action / target identification.

Verified gameplay direction:

- An arithmetic question is active during battle.
- Multiple descending enemies carry different answer values.
- One enemy corresponds to the correct answer.
- The player attacks enemies directly.
- Correct and incorrect targets have different gameplay consequences and score values.

Campaign moment:

**Calculate -> identify the correct answer-bearing enemy -> shoot it -> see the wave resolve.**

Do not depict this as a passive quiz followed by an unrelated attack animation.

### Math Rain

Campaign role: speed, pressure, and consequence.

Verified gameplay direction:

- Math problems descend as raindrops.
- The player selects answer cards.
- Correct selection resolves the matching falling problem and builds score/combo.
- An incorrect selection resets combo and pushes unresolved raindrops closer to danger.
- Missed problems cost lives.

Campaign moment:

**Calculate -> choose the answer under time pressure -> immediately change the falling threat.**

### Memory Game

Campaign role: observation, recall, and competitive choice.

Verified gameplay direction:

- Players flip two cards and try to find matching pairs.
- A successful match scores a pair and keeps the turn.
- A failed match passes the turn.
- The game supports human-vs-human and AI play.
- A limited hint system can temporarily reveal a pair.

Campaign moment:

**See -> remember -> choose the two remembered positions -> complete the pair.**

### Math Defender

Campaign role: the clearest strategic expression of the FiveRocks design philosophy.

Current product/design direction:

- The stage loop is Problem -> Scout -> Preparation -> Battle -> Result.
- Correct math answers earn preparation currency rather than directly multiplying damage.
- Scout exposes useful enemy information.
- Preparation converts earned currency into player-selected hero summons/deployment.
- Battle resolves from those choices; math result alone must not determine victory.

Current implementation status must be treated carefully:

- A first playable vertical slice has been merged to the development repository's main baseline.
- Long-term GameBible progression features must not be depicted as implemented unless separately verified.

Campaign moment:

**Solve -> earn resources -> inspect the enemy -> choose/deploy heroes -> watch the choice matter in battle.**

### Match Fix

Campaign role: deliberate puzzle beat and visual metaphor for "thinking changes the game state."

Verified/current development direction:

- The player repairs an incorrect matchstick equation by moving the configured exact number of matchsticks.
- The resulting equation must be mathematically valid and satisfy the move constraint.
- Higher-difficulty content includes exact-two-move puzzles and division.
- Current metagame work includes difficulty packs, hint economy, mastery, sharing, and Infinite Mode.
- Formal production publication status must be re-checked before describing the game as released.

Campaign moment:

**Inspect the wrong equation -> decide what must move -> physically move a matchstick -> watch the equation become correct.**

## 30-second master direction

The current master structure is approximately:

1. Hook: answer/problem framing
2. Math Fighter: target and shoot
3. Math Rain: answer under falling pressure
4. Memory Game: remember and select
5. Math Defender: earn, analyze, prepare, defend
6. Match Fix: slow down, move the match, solve
7. Rapid multi-game montage: THINK. CHOOSE. ACT.
8. Game Hub collection view
9. FiveRocks Games end card: Play. Think. Grow. + Game Hub CTA

The detailed timing and shot description live in `02-synopsis-and-storyboard.md` and should evolve without duplicating the entire storyboard here.

## Tone and editing

- Gameplay-first rather than classroom-first.
- Fast, energetic pacing for action games; deliberately slower beat for Match Fix.
- Let the viewer see the moment of player judgment.
- Use typography as rhythm and emphasis, not as a substitute for showing the mechanic.
- Prioritize readable gameplay over excessive transitions or visual effects.
- Sound should reinforce action consequences: target hit, correct answer, pair match, deployment, matchstick placement.

## Claims and evidence policy

Do not create campaign claims from memory, homepage summaries, or aspirational design alone.

Before a game appears in the final campaign:

1. Check its current `fiverocks-dev/<game>` repository.
2. Read the project's local source-of-truth documents relevant to gameplay/status.
3. Inspect implementation code or tests for the interaction being filmed when practical.
4. Confirm current playable/release status separately from planned design.
5. Record meaningful discrepancies or production decisions in the campaign production log.

If a visually strong planned feature is not implemented, either omit it or clearly treat it as development footage only when the campaign explicitly intends that framing.

## Production deliverables

Planned campaign artifacts:

- factual game analysis
- master synopsis and storyboard
- game-by-game capture/shot list
- capture evidence and source-build references
- 30-second vertical-first master or equivalent source master
- 15-second cutdown
- 6-second bumper cutdown
- copy/CTA variants
- production and revision log

Exact ad-format specifications should be re-checked against current official Google Ads documentation immediately before export/delivery because platform requirements can change.

## Current decisions

Accepted working decisions:

- Lead with gameplay, not the phrase "educational games."
- Treat Game Hub as the destination where the shared FiveRocks gameplay philosophy can be experienced.
- Use real implemented interaction as the visual evidence for every game.
- Use **THINK. CHOOSE. ACT.** as the current campaign motif.
- Retain **Play. Think. Grow.** as the FiveRocks Games closing brand line.
- Favor "decision becomes action" over generic claims such as "learn while having fun."

## Open work

Next production tasks:

- Create a verified shot list for each game.
- Identify exact development build/version/URL or device used for each capture.
- Decide which games are eligible for the first public ad based on current release/prerelease status.
- Reconcile the current Game Hub title inventory with the campaign title inventory before final edit.
- Define final CTA and landing-page state.
- Produce 15-second and 6-second cutdown maps from the master concept.

## Related documents

- `campaign/README.md` — campaign workspace index
- `campaign/02-synopsis-and-storyboard.md` — current synopsis and 30-second storyboard
- `AGENTS.md` — repository and campaign working rules
