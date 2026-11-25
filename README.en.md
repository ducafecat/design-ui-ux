# Design UI UX — AI Agent Skill for HTML + Tailwind Prototypes

English | [简体中文](README.md)

## Installation

Install with npx. Project-level installation is recommended.

```bash
npx skills add ducafecat/design-ui-ux
```

## Usage workflow

### 1. Automatically search for design directions

Start with a product requirements document (PRD) to give the design a clear focus.

Prompt:

```text
/design-ui-ux Create a mobile UI for Xiaohongshu

Reference:
docs/prd.md
```

![Automatically search for design directions](https://files.ducafecat.com/docs/2026/11/25/1795618228981.png)

### 2. Choose a design direction

If none of the options appeal to you, use this prompt:

```text
Show me another batch
```

![Choose a design direction](https://files.ducafecat.com/docs/2026/11/25/1795618428611.png)

### 3. Build the design

<img src="https://files.ducafecat.com/docs/2026/11/25/1795618786169.png" alt="Reference selection prompt" style="zoom: 50%;" />

Enter the reference ID as your prompt:

```text
B2
```

Confirm the look and feel:

<img src="https://files.ducafecat.com/docs/2026/11/25/1795619134358.png" alt="Look and feel" style="zoom:50%;" />

Prompt:

```text
1
```

Output: `design/index.html`

<img src="https://files.ducafecat.com/docs/2026/11/25/1795620741606.png" alt="Completed design" />

### 4. Lay out the design views side by side

Prompt:

```text
Arrange the views from design/index.html side by side and save them to design/平铺.html
```

Output: `design/平铺.html`

![Design views laid out side by side](https://files.ducafecat.com/docs/2026/11/25/1795620965224.png)

### 5. Explore more variations

You can ask AI to create four homepage designs.

Prompt:

```text
Create one homepage design for each of options 1, 2, 3, and 4, and save them to design/compare.html
```

Output: `design/compare.html`

![Four homepage design variations](https://files.ducafecat.com/docs/2026/11/25/1795619938511.png)

## Requirements

- Installation requires Node.js 22.20 or later, including npm / npx. The final HTML deliverable does not require Node.js.
- Local data search uses Python 3 and only the standard library. Without Python, you can still follow the detailed guidelines, but must not claim to have completed the search.
- The full design workflow requires a browser, real screenshots, and local HTML preview. Ego Lite is preferred by default and requires the `ego-browser` skill to be configured separately. If unavailable, explain the limitation and use an alternative browser according to the skill instructions.
- Authoring requires a tool that can compile Tailwind. The final deliverable should require no Node.js, CDN, or runtime build.

## Feedback, maintenance, and licensing

Read [CONTRIBUTING.md](CONTRIBUTING.md) before submitting improvements. See [CHANGELOG.md](CHANGELOG.md) for version history and [SECURITY.md](SECURITY.md) for sensitive issues. Report reproducible problems through [GitHub Issues](https://github.com/ducafecat/design-ui-ux/issues).

No project license has been specified, so do not assume an open-source license grant. Before publication, the maintainer must confirm the provenance, redistribution rights, and licensing of the code and data. Source records in the data do not constitute redistribution permission. See the [provenance notice](NOTICE.md).
