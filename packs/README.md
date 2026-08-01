# Rule packs

Optional fragments for Code Spots **catalog adoption** or classic **Export/Import**. Each pack is a partial `.csvs` JSON file merged by bookmark `id` into the Primary workspace root.

## Layout (convention)

```
packs/
  onboarding/       # meta-clip + start here
  productivity/     # roadmap, todos ✅❌, concept workflow
  agent-global/     # commit when asked, minimal diff (→ global storage)
  …/
    manifest.json
    shared.fragment.json
```

`manifest.json` may include optional `catalogHint.suggestedRole` (hint only — the team assigns roles in Code Spots).

## Adopt via wizard (recommended)

1. Add this repo to your workspace and set its root role to **Catalog** (Assignment panel 🎯).
2. Set your team repo as **Primary**.
3. Open **Code Spots → Settings (⚙️) → Adopt rules from catalog…** (or command palette).
4. Choose **Clip source**: prefer a pack (`Pack: onboarding`, etc.) over full catalog / Select all.
5. Read **Purpose / When / Adapt** per row; pick target scope (shared / personal / global).
6. Adopt selected → adapt placeholders on Primary → commit Shared via PR.

## Classic import

1. Open your target workspace root in VS Code/Cursor.
2. Code Spots → **Import** (`Ctrl+Alt+I`, Trial/Pro/Team).
3. Select the pack's `shared.fragment.json`.
4. Review merged items in the sidebar.

## Contributing packs

See [CONTRIBUTING.md](../CONTRIBUTING.md). Prefer small, focused packs (`onboarding`, `pr-workflow`, `release-policy`) over one mega-file.
