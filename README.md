<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/oriw-app/oriw-design/main/logo/oriw-wordmark-white.svg">
    <img src="https://raw.githubusercontent.com/oriw-app/oriw-design/main/logo/oriw-wordmark.svg" alt="Oriw" width="240">
  </picture>
</p>

# Oriw templates

Community templates for [Oriw](https://github.com/oriw-app/oriw). Free to use, share and remix, with no attribution needed: everything here is dedicated to the public domain under [CC0 1.0](LICENSE).

Templates in this repository appear in the template gallery inside Oriw.

## Add a template

1. Fork this repository.
2. Create a folder under `templates/` named in lowercase with hyphens, such as `templates/user-story-map`.
3. Add the three files below.
4. Open a pull request. A maintainer checks it opens cleanly and contains no personal or company data.

## Template format

```
templates/<name>/
  template.json   description of the template (below)
  board.oriw      the board itself, exported from Oriw with File > Export > Template
  preview.png     1200 x 800 screenshot of the board
```

`template.json`:

```json
{
  "name": "Retrospective",
  "description": "Went well, to improve and actions, with dot voting.",
  "category": "Meetings",
  "tags": ["agile", "retro", "team"],
  "author": "your GitHub username",
  "minOriwVersion": "0.1.9"
}
```

Categories: Meetings, Planning, Diagrams, Research, Strategy, Education, Fun.

**Status:** the `board.oriw` format is a draft until Oriw 0.1.9 ships. Templates can be proposed now as `template.json` and `preview.png`; the board file follows once export is available.

## Rules

- No personal data, real customer names, or confidential company content.
- Only content you made or have the right to give away. By contributing, you dedicate your template to the public domain under CC0 1.0.
- Keep text short and in plain English; translations are welcome as separate templates.

## Part of Oriw

| Repo | What |
| --- | --- |
| [oriw](https://github.com/oriw-app/oriw) | The app (source opens with the 0.1.9 preview) |
| [oriw-design](https://github.com/oriw-app/oriw-design) | Design system and logo |
| [oriw.app](https://github.com/oriw-app/oriw.app) | Website |
| [oriw-templates](https://github.com/oriw-app/oriw-templates) | Community templates |

- **Roadmap:** [Oriw Roadmap](https://github.com/orgs/oriw-app/projects): what's planned for each release, across all repos.
- **Contribute:** read the [contributing guide](https://github.com/oriw-app/.github/blob/main/CONTRIBUTING.md). Issues use the labels `feature`, `bug`, `docs`, `chore`, `area: …` and `priority: …`.
- **Security:** report problems privately as described in the [security policy](https://github.com/oriw-app/.github/blob/main/SECURITY.md).
