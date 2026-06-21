# GitHub repository settings (maintainer checklist)

Apply these in the GitHub UI for `timejunky/r4it-CodeSpots-Templates`. Files in this repo cannot set all of them.

## General

| Setting | Value |
|---|---|
| **Description** | Companion workspace for Code Spots — shared URLs, AI clip templates, and importable rule packs. Add as a multi-root folder alongside your projects. |
| **Website** | `https://www.ready-4-it.com/en/produktoverview/codespots` |
| **Topics** | `codespots`, `vscode`, `cursor`, `ai`, `bookmarks`, `templates`, `ready-4-it` |
| **Template repository** | Off (this is a companion repo to clone/add, not a “Generate repo from template” seed) |
| **Allow forking** | **On** — required for external pull requests |
| **Wiki** | **Off** — edits only via PR |
| **Issues** | On (requests for new clips / packs) |
| **Sponsorship** | Enabled via `.github/FUNDING.yml` (PayPal + product page) |

## Rules → Rulesets → New branch ruleset

| Field | Value |
|---|---|
| **Name** | `Protect main` |
| **Enforcement status** | **Active** |
| **Target branches** | `main` |
| **Bypass list** | User `timejunky` (and optionally role **Repository admin**) |
| **Require a pull request before merging** | On — required approvals: `0` (solo) or `1` (review others) |
| **Block force pushes** | On |
| **Restrict deletions** | On |
| Everything else | Off (unless you add CI later) |

Maintainers on the bypass list may push directly to `main`; everyone else merges via pull request.

## Collaborators

Keep **Write** access limited to maintainers. Contributors use **fork + PR**.
