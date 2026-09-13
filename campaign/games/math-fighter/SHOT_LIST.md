# Math Fighter Standalone Promo — Shot List

## Capture objective

Capture enough real gameplay to make the mechanic understandable before the edit accelerates.

The must-have evidence chain is:

`problem -> answer-bearing enemies -> player zone choice -> ship movement -> firing -> correct target clear`

The first usable hero shot should contain as much of that chain as possible in one continuous take.

## Build provenance

Before recording, write down:

- development repository: `fiverocks-dev/math-fighter`
- exact 40-character commit SHA
- branch/ref used for capture
- Unity version from `ProjectSettings/ProjectVersion.txt`
- device / emulator / editor target
- screen resolution and orientation
- selected control mode
- selected game mode
- arithmetic operation / stage
- whether the build contains any unmerged PR changes

Current planning baseline at document creation:

`main = 91d3209c61965f3a072271eb947f0650229a64fe`

Do not assume this remains the capture baseline.

PR #108 currently proposes movement-smoothing changes for target-seeking controls. Re-check its merge state before recording and record the exact capture SHA either way.

## Preferred hero control mode

### Three-Zone

Current main behavior makes Three-Zone especially suitable for advertising because the player's decision can map visibly to one of three enemy columns:

1. tap one horizontal screen zone,
2. ship moves toward that zone,
3. once in the selected zone during battle, firing is active,
4. quiz resolution clears the targeting/fire state.

This provides a readable `think -> choose -> move -> fire` chain.

Do not imply that tapping an enemy directly is the mechanic unless the captured build actually behaves that way.

## Must-have shots

### MF-01 — Clean mechanic establishment

**Priority:** Critical

Capture one uninterrupted interaction where:

- arithmetic problem is clearly readable,
- all three enemy answer values are readable,
- correct answer is not already aligned with the ship,
- player makes a visible zone selection,
- ship moves into the correct zone,
- firing begins,
- correct enemy is destroyed,
- wave/quiz visibly resolves.

Target usable duration: 5–8 seconds.

Record multiple takes with different arithmetic problems and correct lanes.

## MF-02 — Left-to-right decision

**Priority:** High

Start with the ship clearly away from the correct answer lane.

Prefer a large horizontal move so the viewer can see that the arithmetic answer changed where the player chose to fight.

Capture both left-to-right and right-to-left variants if practical.

## MF-03 — Rapid correct sequence

**Priority:** High

Capture 3–5 consecutive correct interactions with minimal downtime.

Goal: source material for the acceleration section after the mechanic is established.

Do not sacrifice answer legibility just to create speed.

## MF-04 — Pressure state

**Priority:** High

Capture a valid gameplay moment with enemies noticeably lower on screen before the player resolves the problem.

Goal: communicate that the player is making the calculation while threats are moving.

Avoid a take where overlapping VFX or UI makes the answer values unreadable.

## MF-05 — Best correct-hit payoff

**Priority:** Critical

Capture the cleanest possible correct-target destruction:

- unobstructed projectile path,
- readable enemy answer before impact,
- satisfying destruction/VFX,
- clean wave resolution immediately afterward.

This is the preferred end-card transition shot.

## MF-06 — Incorrect target consequence

**Priority:** Optional

Capture one deliberate wrong-target attack only if it can be done without creating misleading footage.

Purpose:

- possible contrast in the long master,
- demonstrate that targets are meaningful rather than cosmetic.

Do not make this a required beat. The ad's main story is understanding and mastery of the mechanic.

## MF-07 — Player damage / danger

**Priority:** Optional

Capture enemy contact / player hit feedback if it reads cleanly.

Use only as secondary tension footage.

Do not imply a life/health rule that is not visible or verified in the captured build.

## MF-08 — Challenge mode escalation

**Priority:** Optional pending build verification

Capture Challenge footage only after confirming current behavior and UI in the exact recording build.

Useful possibilities:

- increasing level display,
- faster or denser battle pacing,
- score progression.

Do not use Challenge footage to imply unverified progression systems.

## UI / setup shots

### MF-09 — Title / lobby

Capture a clean Math Fighter title or current approved lobby identity for the end card / transition.

Do not rely on this as the opening hook.

### MF-10 — Mode selection

Optional supporting footage of Normal / Challenge selection if the standalone campaign later needs feature breadth.

Not required for the first pilot master.

## Recording rules

- Preserve native gameplay readability.
- Record without notification overlays or unrelated debug UI.
- If touch input is not visible in raw capture, record clean gameplay first and add a restrained touch indicator in post rather than modifying runtime UI solely for the ad.
- Avoid fake answer values or staged UI composites that do not correspond to playable behavior.
- Capture several takes for each lane because answer/UI readability may be more important than the visually most dramatic run.
- Keep a few seconds of handle before and after every intended shot for editing and audio transitions.
- Record game audio separately/cleanly where practical so firing, impact, correct resolution, damage, and UI sounds can be emphasized in the edit.

## Vertical composition check

Before the full capture session, perform a short 9:16 test and answer:

- Is the arithmetic problem readable at phone-ad size?
- Are all three answer values readable simultaneously?
- Is the player ship visible without cropping critical bottom UI?
- Is the selected lane understandable?
- Does a touch indicator obscure an answer value?
- Does center-cropping from another aspect ratio remove a lane?

If 9:16 crop damages the three-lane mechanic, prefer capturing or composing from a source that preserves all lanes rather than forcing an aggressive crop.

## Capture matrix

At minimum, collect:

| Take | Correct lane | Pressure | Purpose |
|---|---|---|---|
| A | Left | Low | mechanic establishment |
| B | Center | Low | clean alternate |
| C | Right | Low | mechanic establishment |
| D | Opposite current ship position | Medium | obvious movement choice |
| E | Any | High | pressure beat |
| F | Mixed sequence | Rising | rapid montage |

For each take, record the exact problem and answer values in the production log so editors can verify the on-screen logic later.

## Acceptance criteria for the first capture session

The session is sufficient to begin editing when all of the following are available:

- at least two clean complete decision chains,
- at least one large visible lane change into the correct target,
- at least one 3+ answer rapid-success sequence,
- at least one pressure-state success,
- at least one strong final impact/clear,
- a clean title/end-card source,
- exact build provenance recorded.

## Post-capture review questions

Immediately after capture, review at actual mobile ad size rather than only on a desktop monitor.

Record whether:

1. the viewer can solve/read the first problem,
2. the correct enemy is visually identifiable before the player moves,
3. movement clearly communicates a choice,
4. firing looks player-driven rather than automatic/unrelated,
5. correct-target resolution is obvious,
6. the footage survives 9:16 presentation,
7. the first full interaction can fit inside roughly 6–8 seconds without losing comprehension.
