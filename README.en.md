# Design UI UX — AI Agent Skill for HTML + Tailwind Prototypes

English | [简体中文](README.md)

An Agent Skill for developers and product teams creating mobile or desktop UI/UX prototypes. It combines real template references, step-by-step style interviews, and a self-contained HTML + Tailwind deliverable.

The default output is `design/index.html`, containing business views, interactions, embedded assets, and a style guide. This repository is in initial preparation: no remote publication, catalog listing, or cross-client compatibility is claimed.

## Workflow

1. Define the product, target device, and page scope.
2. Review at least five template sources and present six real screenshots in `design/preview.html` per round.
3. Select a reference, interview one question at a time, and confirm the style.
4. Build one HTML file with compiled Tailwind CSS, scripts, assets, and a style guide embedded.
5. Verify the file in an isolated directory using `file://`, recording checks and limitations.

Small changes follow existing conventions. Users can explicitly skip reference selection or interviews.

## Install into a project

From a local copy of this repository:

```bash
mkdir -p /absolute/path/to/your-project/.agents/skills
cp -R skills/design-ui-ux /absolute/path/to/your-project/.agents/skills/
```

Replace the destination path. Back up and compare any existing installation before updating. Ask an Agent Skills-capable client to read `.agents/skills/design-ui-ux/SKILL.md`. Discovery rules vary by client; universal compatibility has not been tested.

Python 3 is needed for optional local search and uses only the standard library. The full workflow needs browser automation, screenshots, and local HTML preview. Ego Lite is preferred and requires a separately configured `ego-browser` skill; the workflow describes fallback behavior. Tailwind compilation is needed during authoring; final HTML should require no Node.js, CDN, or runtime build.

## Example

> Use design-ui-ux to design a mobile fitness booking interface with a course list, details, and booking result. Save outputs in design/.

Expect a requirements summary and reference preview first; after selection and style confirmation, expect `design/index.html` with an embedded style guide. No finished fitness app or booking backend is included.

For a small change:

> Use design-ui-ux to fix form spacing and keyboard focus in design/index.html, following its existing style.

## Search and validation

Run from this repository root:

```bash
python3 skills/design-ui-ux/scripts/search.py "keyboard focus modal" --domain ux
python3 skills/design-ui-ux/scripts/search.py "responsive form navigation" --stack html-tailwind
python3 skills/design-ui-ux/scripts/validate_data.py
```

Search returns candidate recommendations. Validation checks data integrity; neither verifies a generated interface. The skill instructions and detailed references are currently written in Chinese.

## Documentation and maintenance

- [Skill instructions](skills/design-ui-ux/SKILL.md)
- [Design standards](skills/design-ui-ux/references/design-standards.md)
- [Style interview](skills/design-ui-ux/references/style-interview.md)
- [Search guide](skills/design-ui-ux/references/search-guide.md)
- [GitHub publication metadata](docs/github-metadata.md)
- [Contributing](CONTRIBUTING.md), [changelog](CHANGELOG.md), [security](SECURITY.md)

Once a remote repository exists, use its Issues for reproducible feedback. No project license has been selected. Do not assume an open-source grant: the maintainer must confirm code/data provenance, redistribution rights, and licensing before publication. See [NOTICE.md](NOTICE.md).
