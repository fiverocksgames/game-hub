# Match Fix Promotional Video Bootstrap

## Project role

Create a standalone promotional video for **Match Fix** using the current development-repository puzzle rules and playable behavior.

Source project: `fiverocks-dev/match-fix`

## 1. Game as the player experiences it

### Player-facing game definition

Match Fix is a matchstick equation puzzle in which the player starts from an incorrect equation and must move the exact required number of matchsticks to make the equation mathematically correct.

The basic player loop is:

`inspect the wrong equation -> find a possible move -> drag matchstick(s) -> form a valid equation -> solve the puzzle`

Current development direction and implemented domain behavior include:

- The player begins from an incorrect equation built from matchstick-style symbols.
- A puzzle requires moving the configured exact number of matchsticks.
- The final equation must be mathematically valid.
- A valid equation reached with the wrong move count does not satisfy the puzzle constraint.
- Content is organized into multiple difficulty packs.
- Earlier packs focus on exact-one-move puzzles; higher difficulty introduces exact-two-move puzzles.
- Division is present in higher-difficulty content.
- Current metagame work includes hints, mastery records, Daily Spin, sharing, and Infinite Mode.

### What should be obvious to a new player

Within a few seconds, the viewer should understand:

1. the starting equation is wrong,
2. matchsticks can be physically moved,
3. the move count is constrained,
4. the goal is to transform the equation into a correct one.

This section defines **what the puzzle is and what the player does**.

## 2. Product / design intent

The design combines arithmetic validity with spatial transformation.

Important design characteristics include:

- the player reasons about both numbers/operators and physical matchstick geometry,
- exact move count is part of the puzzle rule, not just a scoring bonus,
- the solution is expressed through direct manipulation rather than selecting an answer from a list,
- higher difficulty expands the search space through more complex move constraints and operators,
- the before/after equation state gives immediate visual confirmation of the reasoning result.

The satisfying transformation is a consequence of the puzzle design, but the game should first be described as an **exact-move matchstick equation puzzle**.

Formal production/publication status must be re-checked before final advertising language.

## 3. Promotional strategy

### Current promotional hook

Working hook:

**Move the match. Make it true.**

Alternative Korean framing:

**성냥을 옮겨, 식을 완성하라.**

The strongest visual chain is:

`wrong equation -> inspect -> select matchstick -> move -> correct equation`

### Campaign experience to communicate

Priority order:

1. Make the viewer immediately recognize that the equation is wrong.
2. Show that the player can physically move a matchstick.
3. Make the exact-move rule understandable.
4. Show the equation becoming mathematically correct as the payoff.
5. Escalate later to more surprising transformations, exact-two-move puzzles, or timed play if verified.

## Hero footage

Priority capture moments:

1. A visually simple incorrect equation readable in under one second.
2. A deliberate pause while the player studies it.
3. One matchstick being selected and dragged.
4. The destination position clearly visible before placement.
5. Matchstick drop producing a valid equation and success feedback.
6. A second puzzle showing a different transformation.
7. Optional exact-two-move puzzle for escalation.
8. Optional Infinite Mode countdown/rapid solving only if current playable status is verified.

## Creative rhythm

Recommended standalone video rhythm:

`SEE WRONG -> THINK -> MOVE -> CHECK -> SOLVED -> HARDER PUZZLE`

Unlike Math Fighter or Math Rain, this video should embrace anticipation and clarity. The physical placement should be the sensory payoff.

## Visual identity hypothesis

- Minimal, deliberate camera/edit movement.
- Keep the equation large and readable.
- Emphasize cursor/hand motion and exact placement.
- Use subtle tension sound before the move, then a crisp placement/success sound.
- Favor understandable transformations before clever rapid montage.

## Claims to avoid without re-verification

Do not claim without current verification:

- formal public release/production status,
- exact total puzzle count if content inventory changes,
- all metagame systems as generally available if still prerelease,
- educational efficacy or quantified reasoning improvement,
- that every puzzle has a unique solution unless current validation explicitly guarantees it.

## Candidate taglines

Game-explaining options:

- **Move the match. Make it true.**
- **Fix the equation in the exact number of moves.**
- **성냥을 옮겨, 식을 완성하라.**

Transformation/escalation options:

- **Move one thing. Change the whole equation.**
- **See the equation differently.**
- **하나를 옮기면 식 전체가 달라진다.**

These are working creative options, not approved final copy.

## Recommended first deliverable

Create a 20-25 second standalone synopsis/storyboard with this order:

`explain core exact-move puzzle -> satisfying first solve -> harder transformation -> optional speed/escalation beat`

## Re-verification before production

Before final capture, re-check:

- current `docs/PROJECT_STATUS.md` and repository-local working instructions,
- puzzle candidate/equation validation domain code and tests,
- exact move-count rules for selected footage,
- current pack inventory and Infinite Mode state,
- current prerelease/production publication status,
- exact build or preview URL used for footage.
