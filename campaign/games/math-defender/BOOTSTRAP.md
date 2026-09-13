# Math Defender Promotional Video Bootstrap

## Project role

Create a standalone promotional video for **Math Defender** that communicates its strategy-RPG identity and the relationship between math performance and tactical agency.

Source project: `fiverocks-dev/math-defender`

## Evidence-grounded game definition

Math Defender is an educational strategy RPG whose stage structure connects math, scouting, preparation, and defense.

Current canonical stage loop:

`Problem -> Scout -> Preparation -> Battle -> Result`

Current vertical-slice direction:

- A stage presents math questions one at a time.
- Correct answers grant preparation currency.
- Incorrect answers do not immediately fail the stage.
- Scout reveals enemy composition and meaningful tactical traits.
- The player spends earned currency to summon/deploy heroes.
- Heroes are intended to be functionally distinct, not merely cosmetic variants.
- Battle resolves from the player's chosen setup.
- Math result alone must not determine victory; hero choice and deployment must matter.
- Result connects math performance, spending, and battle outcome.

A first playable vertical slice has been merged to the development repository's main baseline. Long-term GameBible progression should not be shown as already implemented without separate verification.

## Core promotional hook

**Solve for options. Win with strategy.**

Alternative Korean framing:

**문제를 풀어 힘을 얻는 게 아니라, 선택지를 얻는다.**

The strongest conceptual chain is:

`solve -> earn -> scout -> choose -> deploy -> defend`

## Audience experience to communicate

The viewer should understand that:

1. math creates resources and strategic possibility,
2. the player must read the enemy before committing resources,
3. the important decision is which hero to deploy and where,
4. the resulting battle proves whether that choice worked.

## Hero footage

Priority capture moments:

1. A correct answer visibly increasing preparation currency.
2. Scout revealing enemy type/count plus one meaningful trait.
3. Two tactically distinct hero choices visible at the same time.
4. Player dragging/selecting and deploying a hero to a legal position.
5. Start Battle transition.
6. Automatic battle where the chosen setup visibly succeeds or struggles.
7. Result screen connecting math accuracy, economy, and battle result.

A particularly strong comparison shot would hold the same stage and math result constant while showing two different preparations producing visibly different outcomes, if current build support and capture time allow it.

## Creative rhythm

Recommended standalone video rhythm:

`SOLVE -> READ THE ENEMY -> BUILD YOUR PLAN -> WATCH IT PLAY OUT`

This video should be slower and more strategic than Math Fighter or Math Rain. Do not cut so rapidly that Scout and Preparation become unreadable.

## Visual identity hypothesis

- Tactical, deliberate pacing.
- Emphasize information hierarchy: currency, enemy trait, hero roles, placement.
- Use battle payoff as the visual climax rather than the math-answer animation.
- Avoid framing summoned heroes as literal towers in player-facing copy or graphics.

## Claims to avoid without re-verification

Do not depict or claim as current gameplay unless separately verified:

- world-map progression,
- broad job/class trees,
- full equipment/meta economy,
- challenge-tower or ranking systems,
- long-term story progression,
- any GameBible feature not present in the captured build.

Do not simplify the game to `correct answer -> more attack power`; this contradicts the project's core economy principle.

## Candidate taglines

- **Solve. Scout. Deploy. Defend.**
- **Math gives you options. Strategy wins the battle.**
- **Earn the plan. Build the defense.**
- **풀어서 얻고, 보고 판단하고, 배치해서 막아라.**

These are working creative options, not approved final copy.

## Recommended first deliverable

Create a 25-30 second standalone synopsis/storyboard centered on one full stage decision chain from Problem through Battle, with Result as the payoff.

## Re-verification before production

Before final capture, re-check:

- `README.md`, `Docs/PROJECT_CHARTER.md`, `Docs/GameBible/`, and `Docs/Project/HANDOFF.md`,
- current vertical-slice design/status documents,
- current implementation of currency, Scout, hero placement, Battle, and Result,
- exact playable Android/build state used for footage.
