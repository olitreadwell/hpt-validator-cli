# CMSgov/hpt-validator-cli context
> refreshed 2026-09-03 | upstream default: main @ 5a6a155

## Identity & policies
- upstream: CMSgov/hpt-validator-cli, default branch `main`, primary language TypeScript, English-first (yes — all docs/UI in English)
- CLA/DCO: none (CONTRIBUTING has no CLA/signup; contributions released under CC0)
- AI-assisted PR policy: unstated (no mention in CONTRIBUTING)
- signed commits required: no (no branch protection on main)
- PR template: `.github/PULL_REQUEST_TEMPLATE.md` (One line description / Problem / Solution / Result / Test Plan)
- external tracker: github

## Conventions (verified from merged PRs)
- branch naming: mixed — `version-bump*` (dominant), `feature/...`, `build/...`, `readme-versions`, `daniel-eckel-data-dictionary-link`; no single strict pattern
- commit style: plain imperative / short subjects (e.g. "grabbing v2.5.0 validator", "Add version output command")
- test command: `npm run lint` (tsc + eslint), `npm run prettier`; CI = lint + prettier on push/PR
- how outside PRs get merged: responsive; small doc/version PRs merged regularly

## Maintainer picture
- active maintainers: CMS open-source team; responsive to small doc/version PRs
- areas actively worked: validator core version bumps, README updates

## Issue-area health
- no open PRs; issues mostly dependency bumps and version-choice requests

## Gap ledger (dedupe — READ FIRST, never re-pick)
- `2026-09-03` self-found trivial cleanup (README broken contributors link, README "within in" duplicate word, README JSON output example stale field names, SECURITY.md email link stray period) — outcome: pr-opened (https://github.com/olitreadwell/hpt-validator-cli/pull/1) — lesson: docs-only, verified against live CLI output; no upstream PR touches these strings

## Mined gaps (discovered, not yet attempted)
- none
