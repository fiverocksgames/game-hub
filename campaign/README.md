# Game Hub Campaign Workspace

This directory contains campaign planning and production documents for Game Hub promotion and standalone promotional-video projects for individual FiveRocks Games titles.

## Campaign roadmap

- Production roadmap: `ROADMAP.md`
- Current sequence: Math Fighter standalone pilot -> Game Hub brand film -> remaining standalone videos -> production-template standardization

The roadmap defines **when to validate and standardize the production process**. It should not be treated as a requirement that all videos share the same creative treatment.

## Game Hub brand campaign

- Canonical brief: `CAMPAIGN.md`
- Current campaign: Google Ads brand video for Game Hub
- Working branch: `campaign/google-ads-brand-video`

Supporting documents:

- `01-game-analysis.md` — factual gameplay analysis based on development repositories
- `02-synopsis-and-storyboard.md` — Game Hub campaign synopsis and 30-second storyboard
- `03-shot-list.md` — capture requirements by game
- `04-copy-and-variants.md` — ad copy and short-form variants
- `05-production-log.md` — production decisions, evidence, and revision notes

## Standalone game campaigns

Individual game promotional-video projects live under `games/` and are intentionally separate from the Game Hub multi-game brand film.

- `games/math-fighter/BOOTSTRAP.md`
- `games/math-defender/BOOTSTRAP.md`
- `games/math-rain/BOOTSTRAP.md`
- `games/memory-game/BOOTSTRAP.md`
- `games/match-fix/BOOTSTRAP.md`

See `games/README.md` for the per-game campaign workflow and expected document structure.

## Working principle

Campaign documents should be grounded in the current FiveRocks Games development repositories and actual implemented gameplay. Public website marketing copy is not treated as the primary source for game behavior.

Before finalizing footage or claims for an individual title, re-check the corresponding `fiverocks-dev/<game>` repository and record the exact playable/build state used for capture.
