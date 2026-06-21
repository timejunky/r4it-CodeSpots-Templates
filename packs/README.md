# Rule packs

Optional fragments for Code Spots **Export/Import**. Each pack is a partial `.csvs` JSON file merged by bookmark `id` into the active workspace root.

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

## Import today

1. Open your target workspace root in VS Code/Cursor.
2. Code Spots → **Import** (`Ctrl+Alt+I`, Trial/Pro/Team).
3. Select the pack's `shared.json` fragment.
4. Review merged items in the sidebar.

## Import later (roadmap)

Dedicated “Import clip pack” with target scope (shared / personal / global) without full workspace overwrite.

## Contributing packs

See [CONTRIBUTING.md](../CONTRIBUTING.md). Prefer small, focused packs (`onboarding`, `pr-workflow`, `release-policy`) over one mega-file.
