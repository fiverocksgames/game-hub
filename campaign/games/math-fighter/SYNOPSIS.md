# Math Fighter Standalone Promo — Synopsis

## Role in the campaign roadmap

Math Fighter is the first standalone promotional-video pilot.

The purpose of this pilot is twofold:

1. produce a useful Math Fighter promotional video,
2. learn which parts of the production process can later be reused for the Game Hub brand film and other standalone game campaigns.

Do not treat choices made for Math Fighter as universal campaign rules until they have been tested against the multi-game Game Hub film.

## Product truth

Math Fighter is a math-action shooting game in which the active arithmetic problem determines which descending enemy should be attacked.

For the current Three-Zone control mode, the player taps one of three horizontal screen zones. The ship moves toward that zone and fires while positioned in the selected zone during active play.

The core player-readable chain is:

`read problem -> calculate answer -> find the enemy carrying that answer -> choose its zone -> move/fire -> resolve the wave`

This is not a quiz followed by a decorative combat animation. The arithmetic answer is used to make the combat decision itself.

## Player view

From the player's perspective:

- an arithmetic problem is active,
- three enemies descend with different answer values,
- the player calculates the answer,
- the player identifies which enemy carries that value,
- the player moves the ship into that enemy's lane/zone,
- the ship fires,
- hitting the correct target advances the quiz/wave,
- mistakes and enemy contact have gameplay consequences.

The video should make this understandable without requiring narration.

## Design intent

The interesting design idea is not simply "practice arithmetic faster."

Math Fighter tries to turn arithmetic into an action-game targeting decision. The calculation is useful because it tells the player where to move and what to attack.

The intended feeling is:

**I solved it, I saw the target, I moved, and I hit it.**

Speed matters because the enemies continue descending while the player thinks and acts.

## Promotional proposition

Primary working proposition:

**정답을 고르는 게 아니라, 정답을 격추한다.**

Working English equivalent:

**Find the answer. Hit the target.**

This is a promotional framing of the verified interaction, not a replacement for the complete game definition.

## Story premise

Open directly inside a battle.

A problem appears. Three enemies descend with plausible answers. Give the viewer just enough time to solve it too.

The ship is not yet aligned with the correct target.

The player taps the correct zone. The ship crosses into position and begins firing. The correct enemy is destroyed and the wave resolves.

Now that the audience understands the rule, accelerate. Show two or three faster decisions: problem, answer, zone, fire, clear. Increase visual pressure through descending enemies and faster cuts rather than through explanatory copy.

Use a mistake or danger moment only if it improves comprehension. The central story is mastery of the core interaction, not punishment for being wrong.

Finish on a clean combat payoff and Math Fighter identity/CTA.

## Emotional arc

`WHAT IS THIS? -> I GET IT -> I CAN SOLVE IT -> MOVE -> HIT -> AGAIN, FASTER`

The first successful interaction is the explanatory moment.

The later interactions are the excitement/payoff.

## Recommended master length

Target a **20–25 second standalone master** for the pilot.

Reasoning:

- the first 5–8 seconds need enough readability for a new viewer to understand problem -> target -> movement -> attack,
- the middle can accelerate once the mechanic is understood,
- the ending should leave room for title/CTA without turning the piece into a tutorial.

A 15-second cut and 6-second bumper should be derived from the master after the first edit proves which shots remain understandable at shorter durations.

## Creative guardrails

- Gameplay comes before educational-benefit claims.
- Show the player's decision; do not cut from problem directly to enemy explosion.
- Keep problem and enemy answer values readable.
- Do not imply that selecting a quiz answer button triggers an attack.
- Do not describe exact control behavior that is not present in the captured build.
- Do not use planned progression, upgrades, curriculum claims, or release claims without current verification.
- If Three-Zone mode is the hero capture mode, make the lane/zone decision visually understandable without adding fake UI.

## Pilot learning questions

The postmortem should answer:

1. How many seconds are required before a cold viewer understands the mechanic?
2. Is raw gameplay readable enough in 9:16, or is crop/reframing required?
3. How much on-screen copy improves comprehension before it begins to obscure gameplay?
4. Is visible touch/tap indication needed in the edit to communicate the zone decision?
5. Can one capture session efficiently supply the 20–25s master, 15s cut, and 6s bumper?
6. Which sound cues best communicate decision -> action -> consequence?
7. Which parts of this workflow are reusable for non-action games?

## Evidence snapshot

This synopsis was prepared against `fiverocks-dev/math-fighter` main at:

`91d3209c61965f3a072271eb947f0650229a64fe`

Relevant current evidence includes:

- repository `AGENTS.md` product flow and status boundaries,
- battle/enemy/quiz implementation previously analyzed for answer-bearing enemies and quiz resolution,
- `Assets/Scripts/Player/Player.cs` for explicit firing behavior,
- `Assets/Scripts/Player/ThreeZoneMovementController.cs` for three-zone tap, movement, and fire-state behavior.

Open gameplay-related PRs must be checked again immediately before capture. In particular, PR #108 currently changes target-seeking movement smoothness but does not redefine the promotional concept above.
