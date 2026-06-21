# Recommended rules & AI clips

Curated templates for Code Spots **Commands** (✍️). Clips already in this repo live in [`.csvs/shared.json`](../.csvs/shared.json). Copy more from below into your project or team companion repo.

Full marketing copy: [ready-4-it.com — Code Spots](https://www.ready-4-it.com/en/produktoverview/codespots)

## Companion repo pattern

Add a small repo (like this one) as a **second workspace root** next to your code — same idea as a shared deploy/releaser repo. Bookmarks and clips stay in `.csvs/shared.json` for that root; your app repo keeps its own `.csvs/`.

## Scope scale

| Scale | Storage | Typical use |
|---|---|---|
| **Shared** | `.csvs/shared.json` | Team conventions, onboarding, PR templates |
| **Personal** | `.csvs/personal.json` | Agent guardrails, local dev URLs |
| **Global** | Extension global storage | “Commit only when asked”, minimal diff |

## Three layers (do not mix up)

| Layer | What |
|---|---|
| **AI Clip** | Copy on click from Code Spots Commands |
| **Memory projection** (Pro+) | Optional automatic mirror into AI workspace memory |
| **Cursor / Copilot rules** | Global editor settings — not managed by Code Spots |

## Rules catalog (in `.csvs/shared.json`)

All table items **#1–#22** that are AI clips are included in [`.csvs/shared.json`](../.csvs/shared.json). Clips marked **global personal** in the table are shipped here as templates — copy them to Code Spots global storage on your machine.

| # | Label | Memory projection |
|---|---|---|
| 8 | `Roadmap: status symbols` | ✅ workspace (Pro+ example) |
| 9 | `Todos: ✅ ❌ + timestamp` | ✅ workspace |
| — | `Agent todos: ✅ ❌ in session` | ✅ workspace |
| 15 | `AI rules: clip vs memory vs settings` | off (meta-clip) |
| … | release, git, PR, i18n, … | off unless you enable in UI |

**Memory projection:** Clips with `memoryProjection.workspace: true` are examples for Pro+ — enable in the AI Clip editor so the rule stays in AI workspace memory while this folder is open.

## Optional packs

| Pack | Contents |
|---|---|
| `onboarding/` | Start here + three layers meta-clip |
| `productivity/` | #6–9 + agent todos (✅ ❌ ⏳) |
| `agent-global/` | #2, #10, #16 — import into **global** personal |

## Copy-paste examples

### Commit only when asked (global personal)

```text
Create git commits only when explicitly requested.

Before committing: git status, diff, recent log — then a concise message focused on why.
Never push unless asked.
```

### Minimal focused diff (global personal)

```text
When changing code:

- Smallest correct fix only
- Match existing style and conventions
- No drive-by refactors or unrelated edits
- Reuse existing helpers instead of duplicating logic
```

### PR description template (shared)

```text
## Summary
- What changed and why (1–3 bullets)

## Test plan
- [ ] …

## Notes
- Breaking changes / migration / screenshots if UI
```

### Todos with timestamps (shared, docs root)

```text
In todo.md and agent replies for this project:

- Open: ⏳ Short description
- Done: ✅ Short description — YYYY-MM-DD HH:mm
- Blocked/dropped: ❌ Short description — reason

Do not delete completed items — add a timestamp.
Prefix new tasks with ⏳.
```

## Contributing

Send PRs with new clips or packs. See [CONTRIBUTING.md](../CONTRIBUTING.md).
