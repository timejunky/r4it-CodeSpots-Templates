# Contributing

Thank you for improving shared Code Spots clips and templates.

## Workflow

1. **Fork** this repository (forking must stay enabled — see maintainer setup).
2. Create a branch from `main`.
3. Edit `.csvs/shared.json`, docs, or files under `packs/`.
4. Open a **pull request** against `main`.

Direct pushes to `main` are reserved for maintainers (branch ruleset + bypass list).

## What we accept

- AI clips and URL bookmarks that are **generic** and safe to share in Git
- English clip text (translations welcome as separate locale files)
- Scope scale noted in the PR (Shared / Personal / Global — see `docs/recommended-rules.en.md`)
- Fixes to wording, onboarding, and pack structure

## What we reject

- Secrets, tokens, passwords, or internal-only URLs
- Project-specific paths presented as universal rules (unless clearly labeled as examples)
- Executable shell commands that embed credentials
- Wiki-style drive-by edits outside the PR process

## Review criteria

Maintainers check:

1. No credentials or private infrastructure details
2. Sensible scope (shared vs personal vs global)
3. Useful to teams beyond a single project
4. Valid JSON in `.csvs/` files

## Scope scale (short)

| Scale | Storage | Use when |
|---|---|---|
| **Shared** | `.csvs/shared.json` | Team conventions, onboarding, PR templates |
| **Personal** | `.csvs/personal.json` | Machine-specific URLs, agent guardrails for one dev |
| **Global** | Extension global storage | Habits that never change per project |

## Questions

Open an **Issue** for clip requests. Use a PR when you already have text ready.
