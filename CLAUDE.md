# Oriw templates: notes for Claude

This repository holds community templates for the in-app gallery. The format is in the README and `template.schema.json`.

## Rules for this repo

- Everything here is CC0 (public domain). Only accept content the contributor made or may give away.
- No personal data, real customer names or confidential content.
- Each template folder needs `template.json` (valid against the schema), `board.oriw` and `preview.png` at 1200 × 800.
- Keep names under 40 characters and descriptions under 140.

## How we work

This repository uses the **issuewright** plugin from [oriw-app/dev-plugins](https://github.com/oriw-app/dev-plugins), switched on in `.claude/settings.json` and configured in `.claude/issuewright.json`. GitHub issues are the spec; the owner accepts intent, spec and plan; work follows DDD + BDD + TDD with hexagonal architecture and CQS. The full guide is the plugin's `WORKFLOW.md` (the `issuewright` skill). Releases are the milestones in `oriw`; planning happens on the **Oriw Roadmap** project.

## Oriw rules
- **DDD + BDD + TDD, with hexagonal architecture and strict CQS**, as set out in `oriw/docs/ENGINEERING.md` and `oriw/docs/ARCHITECTURE.md`. Here that means template acceptance criteria are written as Given / When / Then, template words match the glossary in `oriw/docs/DOMAIN.md`, and the schema check in CI is the test every template must pass.
- Never commit secrets. Never put salaries, costs, revenue or customer names in a public repository; they belong in `oriw-company`.
- The repositories are the source of truth: designs in `oriw-design/mocks/`, decisions in the repository they affect. Claude artifacts are previews only.
- Commits are authored by the person running the session; keep the trailers the session adds.

## Things Claude gets wrong

- Nothing recorded yet. Add a line here whenever Claude makes the same mistake twice.
