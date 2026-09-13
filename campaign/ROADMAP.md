# Campaign Production Roadmap

## Purpose

This roadmap defines the order in which FiveRocks Games promotional-video production should be validated and standardized.

The goal is not to define a fixed visual template too early. The goal is to learn from real production, validate which parts of the workflow generalize across different games, and only then standardize the reusable process.

## Decision

Use a three-phase path:

1. Produce one standalone game video as a pilot.
2. Use the pilot learnings to produce the multi-game Game Hub brand film.
3. Use both experiences to define the reusable production template for future standalone videos.

This intentionally avoids two failure modes:

- starting with the Game Hub film and mixing general production problems with multi-game brand-film complexity,
- standardizing a workflow after only one game and accidentally turning one game's creative structure into a universal template.

---

## Phase 1 — Standalone Pilot

### Pilot title

**Math Fighter**

### Why Math Fighter first

Math Fighter has a clear and readable interaction chain:

`problem -> calculate -> identify the answer-bearing enemy -> attack -> visible result`

This makes it a strong first project for validating whether the production workflow can communicate a game's real mechanic quickly and clearly.

Compared with other candidates:

- Match Fix has a very strong advertising hook, but its single transformation mechanic may generalize poorly to other games.
- Math Defender expresses the FiveRocks design philosophy especially well, but its multi-step strategic loop is more complex for a first production test.
- Math Rain and Memory Game remain strong follow-up candidates once the workflow is better understood.

### Pilot objectives

The pilot should answer production questions such as:

- How quickly can a first-time viewer understand the game?
- Which gameplay moments are fun to play but difficult to communicate in an ad?
- Which UI elements remain readable in 9:16 video?
- How much context is required before an action becomes understandable?
- How should captions support rather than replace gameplay understanding?
- Which gameplay actions require special capture preparation?
- Can a master edit produce useful 15-second and 6-second derivatives?
- Which sound effects are important for communicating player action and consequence?

### Pilot production cycle

The complete pilot should go through one full production loop:

```text
BOOTSTRAP
-> SYNOPSIS
-> STORYBOARD
-> SHOT_LIST
-> CAPTURE
-> EDIT
-> 15s CUT
-> 6s CUT
-> POSTMORTEM
```

Do not skip the postmortem. The pilot is successful only if the production experience becomes reusable evidence for later work.

### Pilot deliverables

Under `campaign/games/math-fighter/`:

- `BOOTSTRAP.md` — already established product/campaign starting point
- `SYNOPSIS.md`
- `STORYBOARD.md`
- `SHOT_LIST.md`
- `COPY.md`
- `PRODUCTION_LOG.md`
- `POSTMORTEM.md`

Video outputs should include, where practical:

- primary standalone master
- 15-second cutdown
- 6-second bumper
- vertical-first export suitable for Shorts-style placements

Exact ad-platform specifications must be re-verified before final export.

---

## Phase 2 — Game Hub Brand Film

After the Math Fighter pilot, produce the Game Hub multi-game brand film.

### Role of this phase

The Game Hub film is not only a campaign deliverable. It is also a test of whether the production principles discovered in the pilot still work across games with very different pacing and mechanics.

The central question becomes:

> Can different FiveRocks games be presented through a shared creative language without hiding what makes each game distinct?

### Current shared creative hypothesis

**THINK. CHOOSE. ACT.**

This should remain a hypothesis until validated in the edit.

The film should repeatedly show a real chain of:

`understand -> decide -> act -> visible consequence`

but should not force every game into the same rhythm or visual treatment.

### Additional problems to validate

The Game Hub phase must solve issues not present in a single-title video:

- transitions between different genres
- minimum screen time required for each game to remain understandable
- balancing fast and slow gameplay rhythms
- preserving each game's identity inside a shared brand film
- title weighting and selection
- relationship between gameplay footage and FiveRocks brand language
- Game Hub landing-page / CTA alignment
- deciding whether all eligible titles belong in one master asset

### Outputs

Continue the existing Game Hub campaign documents:

- `CAMPAIGN.md`
- `02-synopsis-and-storyboard.md`
- `03-shot-list.md`
- `04-copy-and-variants.md`
- `05-production-log.md`

Add a Game Hub postmortem after production so cross-game findings can be compared with the standalone pilot.

---

## Phase 3 — Remaining Standalone Videos

After the pilot and Game Hub film, continue standalone campaigns for the remaining games.

Current working order:

1. Math Rain
2. Memory Game
3. Math Defender
4. Match Fix

This order is not a hard dependency and may change based on product readiness, capture availability, campaign priority, or release status.

Each game should preserve its own creative identity.

Examples:

- Math Rain: falling-problem survival arcade
- Memory Game: competitive recall and turn control
- Math Defender: math-earned tactical options and defensive planning
- Match Fix: visual/spatial equation transformation

The reusable process should remain common while the visual and narrative treatment stays game-specific.

---

## Phase 4 — Production Template Standardization

Do not finalize the production template immediately after the first pilot.

Standardization should happen after there is evidence from at least:

- one standalone game video, and
- the multi-game Game Hub brand film.

The template should standardize the **production process**, not the appearance of the videos.

A likely reusable structure is:

```text
1. Product Truth
2. Player Experience
3. Design Intent
4. Promotional Hook
5. Hero Interaction
6. Capture Plan
7. Master Story
8. Short-form Cutdowns
9. Platform Adaptation
10. Production Review
11. Postmortem
```

### What should become standardized

Potential reusable standards include:

- evidence verification before claims or capture
- separation of player experience, product intent, and promotional framing
- definition of one or more hero interactions
- shot-list structure
- capture/build provenance
- vertical readability review
- caption and sound review
- master-to-cutdown workflow
- post-production review checklist
- production postmortem format

### What should not become standardized

Avoid forcing:

- identical runtime for every title
- identical narrative arc
- identical typography rhythm
- identical music style
- the `THINK. CHOOSE. ACT.` motif onto every standalone campaign
- identical number of shots or gameplay beats

A shared FiveRocks production system should make different games easier to communicate, not make different games look the same.

---

## Learning loop

Every completed video should leave behind two kinds of knowledge:

### Product-specific knowledge

Keep inside the individual campaign folder:

- which mechanics communicate well
- which footage is difficult to read
- title-specific capture requirements
- proven and rejected hooks
- game-specific copy decisions

### Reusable production knowledge

Promote into the future shared campaign template only after it is observed across multiple projects or clearly generalizable.

Do not elevate a one-off creative solution into a standard without evidence that it transfers.

---

## Current next action

Begin **Math Fighter Phase 1** by creating:

1. `campaign/games/math-fighter/SYNOPSIS.md`
2. `campaign/games/math-fighter/STORYBOARD.md`
3. `campaign/games/math-fighter/SHOT_LIST.md`

Before finalizing these documents, re-verify the current Math Fighter development repository and the exact playable build that will be captured.
