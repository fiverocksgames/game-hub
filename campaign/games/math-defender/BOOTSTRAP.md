# Math Defender Promotional Video Bootstrap

## Project role

Create a standalone promotional video for **Math Defender** using the current development-repository gameplay and validated vertical-slice behavior.

Source project: `fiverocks-dev/math-defender`

## 1. Game as the player experiences it

### Player-facing game definition

Math Defender is a strategy-defense game in which the player solves math problems to earn preparation resources, scouts the incoming enemies, chooses heroes, deploys them, and then watches the defensive battle play out.

The core stage loop is:

`solve problems -> earn preparation resources -> inspect enemies -> choose/deploy heroes -> start battle -> see the result`

Current canonical stage loop:

`Problem -> Scout -> Preparation -> Battle -> Result`

Current vertical-slice behavior includes:

- A stage presents math questions one at a time.
- Correct answers grant preparation currency.
- Incorrect answers do not immediately fail the stage.
- Scout reveals enemy composition and meaningful tactical traits.
- The player spends earned currency to summon/deploy heroes.
- Heroes are intended to be functionally distinct, not merely cosmetic variants.
- Battle resolves from the player's chosen setup.
- Math result alone must not determine victory; hero choice and deployment must matter.
- Result connects math performance, spending, and battle outcome.

### What should be obvious to a new player

Within a few seconds, the viewer should understand:

1. solving math gives the player resources,
2. those resources are spent on hero deployment,
3. the player must inspect the enemy before choosing a setup,
4. battle outcome depends on the strategy chosen.

This section defines the game from the player's point of view.

## 2. Product / design intent

The project's defining design principle is that mathematics should create **strategic agency**, not directly become combat power.

Important design characteristics include:

- correct answers create preparation currency rather than a direct damage multiplier,
- Scout gives information that should influence deployment,
- preparation is a real choice under resource constraints,
- functionally different heroes make matchup and placement matter,
- battle acts as feedback on the player's prior strategic decisions,
- math performance affects the option space, but does not automatically determine victory.

A first playable vertical slice has been merged to the development repository's main baseline. Long-term GameBible progression must remain separate from currently implemented play.

## 3. Promotional strategy

### Current promotional hook

Working hook:

**Solve. Scout. Deploy. Defend.**

Alternative Korean framing:

**풀고, 보고, 배치하고, 막아라.**

The strongest visual chain is:

`correct answer -> resource gained -> enemy information -> hero choice -> deployment -> battle consequence`

### Campaign experience to communicate

Priority order:

1. Explain that solving problems gives the player preparation resources.
2. Show Scout so the viewer understands there is information to act on.
3. Show a real choice between heroes or placements.
4. Use Battle as the payoff that proves the preparation mattered.
5. Only after the core loop is understood, emphasize the deeper philosophy that math creates options rather than direct attack power.

## Hero footage

Priority capture moments:

1. A correct answer visibly increasing preparation currency.
2. Scout revealing enemy type/count plus one meaningful trait.
3. Two tactically distinct hero choices visible at the same time.
4. Player selecting and deploying a hero to a legal position.
5. Start Battle transition.
6. Automatic battle where the chosen setup visibly succeeds or struggles.
7. Result screen connecting math accuracy, economy, and battle result.

If supported by the current build, a strong comparison shot would show the same stage with different preparations leading to visibly different battle results.

## Creative rhythm

Recommended standalone video rhythm:

`SOLVE -> EARN -> SCOUT -> CHOOSE -> DEPLOY -> DEFEND`

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

Game-explaining options:

- **Solve. Scout. Deploy. Defend.**
- **Solve to prepare. Choose how to defend.**
- **풀고, 보고, 배치하고, 막아라.**

Design-philosophy options:

- **Math gives you options. Strategy wins the battle.**
- **문제를 풀어 선택지를 만들고, 전략으로 승부한다.**

These are working creative options, not approved final copy.

## Recommended first deliverable

Create a 25-30 second standalone synopsis/storyboard centered on one complete stage decision chain from Problem through Battle, with Result as the payoff.

## Re-verification before production

Before final capture, re-check:

- `README.md`, `Docs/PROJECT_CHARTER.md`, `Docs/GameBible/`, and `Docs/Project/HANDOFF.md`,
- current vertical-slice design/status documents,
- current implementation of currency, Scout, hero placement, Battle, and Result,
- exact playable Android/build state used for footage.
