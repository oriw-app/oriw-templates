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
