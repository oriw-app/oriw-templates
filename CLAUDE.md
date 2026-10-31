# Oriw templates: notes for Claude

This repository holds community templates for the in-app gallery. The format is in the README and `template.schema.json`.

## Rules for this repo

- Everything here is CC0 (public domain). Only accept content the contributor made or may give away.
- No personal data, real customer names or confidential content.
- Each template folder needs `template.json` (valid against the schema), `board.oriw` and `preview.png` at 1200 × 800.
- Keep names under 40 characters and descriptions under 140.

## Oriw at a glance

Oriw (said OR-ee-w) is a fast, private, open-source whiteboard for Windows, macOS and Linux: boards encrypted on the user's device, collaboration computer to computer with no cloud required, and an AI agent that uses the model the user chooses (Claude, Gemini, Llama on the user's own computer; GitHub Copilot pending a terms check).

Every change is checked against the twelve product principles in the `oriw` README: fast, light, friendly, accessible, the user's data on the user's device, private by default, never lose work, collaborative without a central server, guests first-class, smart help the user controls, open and extensible, fair and honest.

## Repositories

| Repo | Visibility | What lives there |
| --- | --- | --- |
| `oriw` | Private until launch, then public (AGPL-3.0) | The app: Rust crates, Tauri shell (`app/`), TypeScript canvas (`ui/`) |
| `oriw-enterprise` | Private, commercial | Enterprise features that plug into the app |
| `oriw-design` | Public | Design tokens, components, logo |
| `oriw.app` | Public | Website (GitHub Pages) |
| `oriw-templates` | Public (CC0) | Community templates |
| `oriw-company` | Private, never public | Business model, finance, hiring, legal |
| `.github` | Public | Org profile, community files, issue templates |

## How work is planned and picked up

- **Roadmap:** the GitHub project **Oriw Roadmap** at github.com/orgs/oriw-app/projects collects issues from every public repo. **Oriw Internal** (private) holds enterprise and company work.
- **Releases:** milestones in `oriw`: `0.1.9 Public preview` (due 7 Nov 2026), `0.1.10 Polish` (21 Nov), `0.2 Live collaboration`, `0.3 Guests and VS Code`. Website, template and enterprise issues follow the same release names.
- **Labels (same in every repo):** `feature`, `bug`, `docs`, `chore`; `area: …`; `priority: must-have | should-have | nice-to-have`.
- **What to work on:** the earliest open milestone first, `priority: must-have` first, then the lowest issue number. Skip issues assigned to someone else. Run `/next` to find it.
- **One issue per branch:** `feat/<issue>-<slug>`, `fix/<issue>-<slug>` or `docs/<issue>-<slug>`. Pull request body says `Closes #<issue>` and ticks the issue's "Done when" boxes it meets.
- **Cross-repo work:** open an issue in each repo touched and link them ("Part of oriw-app/oriw#12"). Design changes start in `oriw-design`, then flow into `ui/` and the website.
- **Continuing work:** sessions start with no memory. Before stopping, run `/handoff`: it comments on the issue with what is done, what is next and anything blocking. Starting a session on an issue, read the issue and its latest handoff comment first.

## Rules

- Never commit passwords, keys or tokens. CI in `oriw` runs a secret scan; secrets live in GitHub encrypted secrets or the OS keychain.
- Never put salaries, costs, revenue or customer names in a public repo; they belong in `oriw-company`.
- Commits are authored by the person running the session (their git config). Keep the commit message trailers the session adds.
- **The repos are the source of truth.** Designs and mocks go in `oriw-design/mocks/` (HTML plus a PNG); product and technical decisions go in the repo they affect (`oriw/docs/`, `oriw-company/`). Claude artifacts and docs are previews only: copy anything decided into the right repo in the same session.
- Plain, specific English in code comments, docs, issues and UI text. No jargon where a plain word works.
- `main` is protected in every repo: all changes go through a pull request with one approving review, and CI must pass where it exists. Never force-push.
