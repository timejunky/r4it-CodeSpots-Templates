# r4it-CodeSpots-Templates

Companion workspace for [Code Spots](https://www.ready-4-it.com/en/produktoverview/codespots) — shared URLs, starter AI clips, and rule-pack templates you can add alongside your project repos (same pattern as a team tooling repo or deploy helper repo in a multi-root VS Code window).

## Quick use

1. Install [Code Spots](https://marketplace.visualstudio.com/items?itemName=ready-4-it.code-spots) in VS Code or Cursor.
2. Clone this repo (or fork it for your team variant).
3. **File → Add Folder to Workspace…** and add this folder next to your code repos.
4. In Code Spots, assign this root role **Catalog** (Assignment Panel — team decides; not enforced by this repo).
5. Browse clips under this root (copy-on-click) or run **Code Spots → Settings (⚙️) → Adopt rules from catalog…** (or **Assign Files (🎯) → Adopt rules from catalog…**) to copy selected clips into your **Primary** team repo.

Clips here are **reference examples** — they do not automatically become team policy for your code repos. See [catalog adoption concept](https://github.com/timejunky/r4it_code_spot_vs/blob/dev/r4it_code_spot_vs_info/concept.catalog-adoption.en.md) (in the main extension info repo).

**File bookmarks:** This repo ships URL + AI clips only (portable in Git). File bookmarks need absolute `file://` URIs from your machine — add them locally via Code Spots (right-click a file → Add to Category) if you want one-click links to `README.md`, `CONTRIBUTING.md`, etc.

## What is inside

| Path | Purpose |
|---|---|
| `.csvs/shared.json` | **Full starter catalog** — 22 AI clips + URL bookmarks (table #1–22 from recommendations) |
| `docs/recommended-rules.en.md` | Scope legend + copy-paste reference |
| `packs/` | Optional import fragments (`onboarding`, `productivity`, `agent-global`) |
| `.github/` | Funding, PR template, CODEOWNERS, maintainer setup checklist |

**Personal data** (`.csvs/personal.json`) is gitignored — keep credentials and machine-specific URLs there.

## Import a pack (optional)

Use the **Adoption wizard** in Code Spots (Settings ⚙️ or command palette: *Adopt rules from catalog…*) to pick a pack fragment (`onboarding`, `productivity`, `agent-global`) or the full `shared.json`.

Classic **Export/Import** (`Ctrl+Alt+I`) still merges bookmark JSON into the active workspace root. See `packs/README.md` for pack layout and merge-by-id behavior.

## Contribute

External changes go through **fork → branch → pull request**. See [CONTRIBUTING.md](CONTRIBUTING.md).

Maintainers: [`.github/REPOSITORY_SETUP.md`](.github/REPOSITORY_SETUP.md) lists GitHub UI settings (ruleset, forking, description, topics).

## Links

- [VS Code Marketplace](https://marketplace.visualstudio.com/items?itemName=ready-4-it.code-spots)
- [Product overview](https://www.ready-4-it.com/en/produktoverview/codespots)
- [Guides & FAQ](https://www.ready-4-it.com/en/produktoverview/codespots/guides) (language switcher on the site)

Donations: GitHub **Sponsor** button on the repo (via `.github/FUNDING.yml`), not in the sidebar URL list.

## License

Clip text and docs in this repo are provided as reusable templates. Code Spots itself is a commercial product by ready-4-it; see the product page for licensing.
