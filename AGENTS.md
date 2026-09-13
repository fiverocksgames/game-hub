# AGENTS.md

## Purpose

This repository hosts the FiveRocks Games Game Hub and related campaign work.

Agents working in this repository must treat repository evidence as the source of truth and must not infer product behavior, campaign claims, release status, or supported features without evidence.

## Read order

Before making changes, read only the documents relevant to the task, in this order:

1. `AGENTS.md`
2. `README.md`
3. For campaign work, `campaign/CAMPAIGN.md`
4. Other files in `campaign/` that are directly relevant to the requested work
5. Relevant source or deployment files in this repository

When a campaign claim depends on another FiveRocks game, inspect that game's current development repository before relying on public-site marketing copy.

## Source of truth for game behavior

For factual statements about a game's mechanics, implemented features, current development state, or release readiness:

- Prefer the current `fiverocks-dev/<game>` development repository.
- Read the project's own `AGENTS.md`, README, architecture/design documents, requirements, ADRs, handoff/status documents, and implementation code as applicable.
- Prefer implementation code and current canonical project documentation over company-homepage descriptions or earlier campaign copy.
- Distinguish clearly between implemented behavior, validated playable behavior, planned design, prototype behavior, and unreleased work.
- Do not present planned or unverified functionality as currently playable.

Public marketing pages may be used for branding or public-facing naming, but not as the primary authority for gameplay behavior when development-repository evidence is available.

## Campaign workspace

All Game Hub promotional campaign planning and production documentation belongs under `campaign/`.

The campaign's canonical brief is:

- `campaign/CAMPAIGN.md`

Supporting documents may include:

- factual game analysis
- synopsis and storyboard
- shot lists and capture requirements
- copy and ad variants
- production logs
- evidence and revision notes

Keep `campaign/README.md` as a lightweight index. Do not duplicate the full campaign brief there.

## Campaign evidence rules

Every game shown or described in campaign material must be grounded in current repository evidence.

For each claimed gameplay interaction, verify at least one of:

- current implementation code,
- current automated test behavior,
- current canonical game-design documentation that is explicitly implemented or validated,
- current project status/handoff evidence confirming the playable state.

When documentation and code disagree, investigate before writing campaign copy. Do not silently choose the more attractive interpretation.

## Creative rule

The current campaign may use creative framing, editing, typography, music, and sequencing, but it must not invent mechanics.

The intended creative pattern is to show a real chain of:

`understand -> decide -> act -> visible game consequence`

The campaign should demonstrate what the player actually does rather than describe abstract educational benefits that are not directly evidenced by gameplay.

## Status language

Use status wording carefully:

- `released` or `production`: only when repository/release evidence confirms it.
- `playable`: only when a current playable build or validated runtime exists.
- `prototype`, `prerelease`, `in development`: preserve these qualifiers when applicable.
- Planned GameBible or roadmap content must not be filmed or described as already implemented.

## Editing rules

- Keep campaign decisions in Markdown under `campaign/`.
- When a creative direction changes, update `campaign/CAMPAIGN.md` if the change affects the canonical campaign brief.
- Preserve old reasoning in production/revision logs when it has reuse value; do not clutter the canonical brief with obsolete alternatives.
- Prefer small, reviewable commits.
- Do not modify game repositories merely to make campaign footage easier without explicit project-level approval.

## FiveRocks shared policies

When the task touches CI, release, review, deployment, artifacts, runners, or shared operational policy, consult the applicable documents in `fiverocksgames/devops-standards` rather than inventing local policy.

For nontrivial debugging or tooling problems, search `fiverocks-dev/spec-underflow` for relevant Experience Cards before investigation.

For multi-agent orchestration or formal handoff/evidence rules, follow `fiverocksgames/agent-team-os`, beginning with `bootstrap/BOOTSTRAP.md`, and read only the documents needed for the task.

For shared visual/audio/game assets, check `fiverocks-dev/assets` before sourcing or creating replacements, and preserve provenance, license, EULA, and usage restrictions.

## Policy priority

If instructions conflict, use this priority:

1. Explicit Human Project Lead instruction
2. Explicit project policy in the current repository or relevant game's development repository
3. Applicable ATOS governance/evidence/authority rules
4. Applicable `fiverocksgames/devops-standards` policy
5. Campaign workflow or task-level convention

Do not weaken higher-priority safety, authority, provenance, evidence, or fail-closed requirements.