# Memory Game Promotional Video Bootstrap

## Project role

Create a standalone promotional video for **Memory Game** based on its current implemented competitive matching gameplay.

Source project: `fiverocks-dev/memory-game`

## 1. Game as the player experiences it

### Player-facing game definition

Memory Game is a card-matching game in which the player flips cards, remembers where each image is, and tries to collect more matching pairs than the opponent.

The basic player loop is:

`flip cards -> remember positions -> choose two cards -> make a pair -> score -> continue or pass the turn`

Current implementation behavior:

- A player flips up to two cards per turn.
- Matching values score one pair for the current player.
- A successful match keeps the turn.
- A failed match flips the cards back and passes the turn.
- The game ends when all pairs are matched.
- Scores are tracked separately for two players.
- The game supports local human-vs-human and human-vs-AI play.
- AI difficulty options exist.
- Multiple board sizes and card themes are supported.
- A limited hint system can temporarily reveal an unmatched pair.

### What should be obvious to a new player

Within a few seconds, the viewer should understand:

1. cards are hidden and must be remembered,
2. the goal is to find matching pairs,
3. matching scores points,
4. a successful match lets the player keep playing,
5. the game is competitive rather than only a solitary memory exercise.

## 2. Product / design intent

The current design turns memory performance into turn control and score advantage.

Important design characteristics include:

- remembering positions directly improves the player's ability to score,
- a successful pair preserves the player's turn,
- a failed pair transfers control to the opponent,
- score competition creates tension beyond simple completion,
- board size, themes, AI difficulty, and hints vary the challenge without changing the core memory loop.

The turn-retention rule is an important competitive system, but it is not the entire definition of the game.

## 3. Promotional strategy

### Current promotional hook

Working hook:

**See it. Remember it. Match it.**

Alternative Korean framing:

**보고, 기억하고, 짝을 맞춰라.**

The strongest visual chain is:

`cards revealed -> cards close -> remember -> choose two positions -> pair matched -> score`

After the game is understood, the retained-turn rule can become the escalation beat:

`match -> score -> same player goes again`

### Campaign experience to communicate

Priority order:

1. Explain the familiar card-memory interaction immediately.
2. Show that the objective is to collect matching pairs.
3. Make the opponent/score context visible.
4. Then show that a correct memory keeps the turn and creates competitive momentum.
5. Use AI, hints, themes, or board-size variety only as secondary features.

## Hero footage

Priority capture moments:

1. A short reveal of several memorable cards.
2. Cards closing.
3. Player selecting two remembered positions.
4. Successful pair match and score increase.
5. Immediate continuation of the same player's turn.
6. Contrast shot: failed pair, cards close, turn changes.
7. Two-player or AI score race near the end of a board.
8. Optional hint or board/theme variation as secondary footage.

## Creative rhythm

Recommended standalone video rhythm:

`LOOK -> HIDE -> REMEMBER -> PICK -> MATCH -> SCORE -> GO AGAIN`

Use micro-pauses so the audience can try remembering alongside the player.

## Visual identity hypothesis

- Clean, readable card layout.
- Use a short silence or reduced music beat when cards close.
- Match sound and score movement should feel rewarding.
- Competitive framing should be visible through player names/scores/turn indicator when readable.
- Themes can provide color variety, but theme variety should not overwhelm the core memory interaction.

## Claims to avoid without re-verification

Do not claim without current verification:

- quantified memory improvement,
- cognitive-training efficacy,
- online multiplayer,
- matchmaking or network competition,
- unsupported AI sophistication beyond implemented difficulty behaviors,
- final release/platform status not confirmed at production time.

## Candidate taglines

Game-explaining options:

- **See it. Remember it. Match it.**
- **Find the pairs. Beat the opponent.**
- **보고, 기억하고, 짝을 맞춰라.**

Competitive/escalation options:

- **Remember more. Keep the turn.**
- **기억하면, 내 턴이 계속된다.**
- **Memory wins the next move.**

These are working creative options, not approved final copy.

## Recommended first deliverable

Create a 20-25 second standalone synopsis/storyboard with this order:

`core matching mechanic -> score context -> retained-turn advantage -> competitive finish`

## Re-verification before production

Before final capture, re-check:

- current README and `src/domain/game.ts`,
- `src/domain/ai.ts` if AI is featured,
- current board-size/theme configuration,
- current hint behavior and UI,
- exact release/build state used for footage.
