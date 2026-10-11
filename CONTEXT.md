# CMSgov/hpt-validator-cli context
> refreshed 2026-10-11 | upstream default: main @ 5a6a155

## Identity & policies
- upstream: CMSgov/hpt-validator-cli, default branch `main`, primary language TypeScript, English-first (yes — all docs/UI in English)
- CLA/DCO: none (CONTRIBUTING has no CLA/signup; contributions released under CC0)
- AI-assisted PR policy: unstated (no AI/LLM wording in CONTRIBUTING, SECURITY, or .github)
- signed commits required: no (branch protection on main re-checked live 2026-10-11: 404 = none)
- org default: `CMSgov/.github` does not exist (404, re-checked live 2026-10-11) — no inherited org policy
- PR template: `.github/PULL_REQUEST_TEMPLATE.md` (One line description / Problem / Solution / Result / Test Plan)
- external tracker: github

## Conventions (verified from merged PRs)
- branch naming: mixed — `version-bump*` (dominant), `feature/...`, `build/...`, `readme-versions`, `daniel-eckel-data-dictionary-link`; no single strict pattern
- commit style: plain imperative / short subjects (e.g. "grabbing v2.5.0 validator", "Add version output command")
- test command: `npm run lint` (tsc + eslint), `npm run prettier`; CI = lint + prettier on push/PR
- how outside PRs get merged: responsive; small doc/version PRs merged regularly
- issue-first: not required — CONTRIBUTING says small changes may be submitted without an issue

## Maintainer picture
- active maintainers: CMS open-source team; responsive to small doc/version PRs
- areas actively worked: validator core version bumps, README updates

## Issue-area health
- no open issues (2026-10-11)
- 2 open upstream PRs, both code-only: #55 `Add option for debug output` (src/index.ts), #56 `Break long lists of errors into chunks` (src/commands.ts) — no docs/CONTRIBUTING overlap

## Gap ledger (dedupe — READ FIRST, never re-pick)
- `2026-09-03` self-found trivial cleanup (README broken contributors link, README "within in" duplicate word, README JSON output example stale field names, SECURITY.md email link stray period) — outcome: pr-opened (https://github.com/olitreadwell/hpt-validator-cli/pull/1) — lesson: docs-only, verified against live CLI output; no upstream PR touches these strings

## Mined gaps (discovered, not yet attempted)
- `2026-10-11` CONTRIBUTING.md L4 `https://code.gov/` 301s into `digital.gov/resources/...-open-source-software/` which 404s (verified with a real request); replacement `https://digital.gov/topics/open-source` returns 200 — status: attempted (this run)
- `2026-10-11` CONTRIBUTING.md L24 `https://guides.github.com/introduction/flow/` is the retired guides host (301 → docs.github.com); canonical URL `https://docs.github.com/get-started/using-github/github-flow` returns 200 — status: attempted (this run)
- `2026-10-11` README.md L14 pairs `Node (version 20.x)` with `NPM (version 8.5.x)` after commit 0ed86e0 bumped Node 16 -> 20 but left npm; the committed lockfile is lockfileVersion 3 — candidate, not used: the correct npm floor is a judgement call
- `2026-10-11` exhaustive re-hunt found no other genuine trivial errors: codespell/cspell clean (only proper noun "cmsgov"), no doubled words, no UK/US variant mixing, all remaining doc links 200 or anti-bot 403, README help block and JSON example otherwise match live CLI output
