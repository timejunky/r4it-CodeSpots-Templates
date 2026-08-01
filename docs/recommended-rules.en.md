# Recommended rules & AI clips

Curated templates for Code Spots **Commands** (✍️). Clips already in this repo live in [`.csvs/shared.json`](../.csvs/shared.json).

**Public catalog:** [github.com/timejunky/r4it-CodeSpots-Templates](https://github.com/timejunky/r4it-CodeSpots-Templates)

Full marketing copy: [ready-4-it.com — Code Spots](https://www.ready-4-it.com/en/produktoverview/codespots)

## Companion repo pattern

Add this repo as a **second workspace root** next to your code. Assign role **Catalog** in Code Spots. Clips stay reference-only until you adopt them into your **Primary** root.

## How to adopt (recommended)

1. Prefer a **pack** (`onboarding`, `productivity`, `agent-global`) or cherry-pick a few clips — not Select all.
2. Read each row’s **Purpose / When / Adapt** in the wizard Explanation column.
3. Choose **Target**: Shared (team Git) · Personal (you on this root) · Global (you everywhere, Pro).
4. After adopt: replace placeholders (paths, test commands, repo names), commit Shared via PR.
5. Optional Pro: enable memory projection (W/R) on Primary per clip — never copied by the wizard.
6. **Cleanup:** delete unused clips on Primary (+ Git). No special un-adopt API.

## Scope scale

| Scale | Storage | Typical use |
|---|---|---|
| **Shared** | `.csvs/shared.json` | Team conventions, onboarding, PR templates |
| **Personal** | `.csvs/personal.json` | Agent guardrails, local experiments |
| **Global** | Extension global storage | “Commit only when asked”, minimal diff |

## Three layers (do not mix up)

| Layer | What |
|---|---|
| **AI Clip** | Copy on click from Code Spots Commands |
| **Memory projection** (Pro+) | Optional automatic mirror — enable on Primary after adopt |
| **Cursor / Copilot rules** | Global editor settings — not managed by Code Spots |

## Rules catalog (in `.csvs/shared.json`)

Clip `comment` fields carry adoption guidance:

`Shared #N — Purpose: … When: … Adapt: …`

| # | Label | Typical target |
|---|---|---|
| 15 | `AI rules: clip vs memory vs settings` | Shared |
| 20 | `Onboarding: start here` | Shared |
| 8 | `Roadmap: status symbols` | Shared (docs) |
| 9 | `Todos: ✅ ❌ + timestamp` | Shared (docs) |
| 10 | `Git: commit when asked` | Global |
| 16 | `Code: minimal focused diff` | Global |
| … | release, PR, i18n, … | see comments in `shared.json` |

## Optional packs

| Pack | Contents |
|---|---|
| `onboarding/` | #20 + #15 |
| `productivity/` | #6–9 + agent todos |
| `agent-global/` | #2, #10, #16 — usually target **Global** |

## After adopt

- Treat adopted text as a **template** — adapt before relying on it.
- Put clips on the workspace root where the files they mention live.
- If you adopted too much: delete extras on Primary and commit.
