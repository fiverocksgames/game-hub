# Memory Game Promotional Video Bootstrap

## Project role

Create a standalone promotional video for **Memory Game** that emphasizes recall, turn pressure, and competitive play rather than presenting it as a generic solitary memory exercise.

Source project: `fiverocks-dev/memory-game`

## Evidence-grounded game definition

Memory Game is a browser-based competitive matching game built around remembering card positions.

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

The important promotional distinction is that memory is not only a passive cognitive exercise; it creates a competitive advantage because a successful recall lets the player keep control of the turn.

## Core promotional hook

**Remember more. Keep the turn.**

Alternative Korean framing:

**기억하면, 내 턴이 계속된다.**

The strongest visual chain is:

`see cards -> cards close -> remember positions -> choose pair -> match -> score -> keep turn`

## Audience experience to communicate

The viewer should understand that:

1. the player must retain card positions,
2. a correct memory produces an immediate competitive reward,
3. turns and score create tension beyond simple pair matching,
4. the game can be played against another person or AI.

## Hero footage

Priority capture moments:

1. A short reveal of several memorable cards.
2. Cards closing before the audience has fully processed them.
3. Player selecting two remembered positions.
4. Successful pair match and score increase.
5. Immediate continuation of the same player's turn.
6. Contrast shot: failed pair, cards close, turn changes.
7. Two-player or AI score race near the end of a board.
8. Optional hint reveal as a secondary feature, not the main hook.

## Creative rhythm

Recommended standalone video rhythm:

`LOOK -> HIDE -> REMEMBER -> PICK -> MATCH -> KEEP GOING`

This video should use micro-pauses. The audience needs enough time to attempt remembering alongside the player; excessive cutting would remove the appeal of the mechanic.

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
- unsupported AI sophistication beyond the implemented difficulty behaviors,
- final release/platform status not confirmed at production time.

## Candidate taglines

- **See it once. Remember it when it matters.**
- **Match it. Score it. Keep your turn.**
- **Memory wins the next move.**
- **보고, 기억하고, 먼저 맞춰라.**
- **기억한 사람이 한 번 더 한다.**

These are working creative options, not approved final copy.

## Recommended first deliverable

Create a 20-25 second standalone synopsis/storyboard using one miniature competitive story: reveal -> recall -> successful pair -> retained turn -> score race -> final pair.

## Re-verification before production

Before final capture, re-check:

- current README and `src/domain/game.ts`,
- `src/domain/ai.ts` if AI is featured,
- current board-size/theme configuration,
- current hint behavior and UI,
- exact release/build state used for footage.
