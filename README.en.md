# Design UI UX — AI Agent Skill for HTML + Tailwind Prototypes

English | [简体中文](README.md)

Build UI/UX prototypes with HTML + Tailwind. Start with design references, choose a style, and create pages you can preview in your browser.

## Installation

Install with npx, preferably in your project:

```bash
npx skills add ducafecat/design-ui-ux
```

## How to use

### 1. Find design references

Prepare a product requirements document (PRD) describing what you want to build, who it is for, and which pages you need. Then enter:

```text
/design-ui-ux Design a Xiaohongshu-style mobile UI

Reference:
docs/prd.md
```

![Automatically search for design directions](https://files.ducafecat.com/docs/2026/11/25/1795618228981.png)

### 2. Choose a design direction

Pick a direction from the results. If none feel right, ask for more:

```text
Show me another batch
```

![Choose a design direction](https://files.ducafecat.com/docs/2026/11/25/1795618428611.png)

### 3. Create the prototype

<img src="https://files.ducafecat.com/docs/2026/11/25/1795618786169.png" alt="Reference selection prompt" style="zoom: 50%;" />

Enter the ID of your chosen reference, for example:

```text
B2
```

Next, choose from the suggested styles:

<img src="https://files.ducafecat.com/docs/2026/11/25/1795619134358.png" alt="Look and feel" style="zoom:50%;" />

For example, select option 1:

```text
1
```

The prototype is saved to `design/index.html`. Open it in your browser to preview it.

<img src="https://files.ducafecat.com/docs/2026/11/25/1795620741606.png" alt="Completed design" />

### 4. View the pages side by side

To see all the pages together, enter:

```text
Arrange the views from design/index.html side by side and save them to design/平铺.html
```

The result is saved to `design/平铺.html`:

![Design views laid out side by side](https://files.ducafecat.com/docs/2026/11/25/1795620965224.png)

### 5. Compare designs

If you are unsure which style to choose, try a homepage in each style and compare them:

```text
Create one homepage design for each of options 1, 2, 3, and 4, and save them to design/compare.html
```

The result is saved to `design/compare.html`:

![Four homepage design variations](https://files.ducafecat.com/docs/2026/11/25/1795619938511.png)

## Requirements

- Installation needs Node.js 22.20 or later, with npm / npx. The generated HTML pages do not need Node.js.
- Local data search needs Python 3, with no third-party packages. Without Python, you can still build pages using the design guidelines, but local search is unavailable.
- Finding references and checking pages needs a browser that supports screenshots and local HTML previews. Ego Lite is the default and needs the `ego-browser` skill configured separately. You can also use another browser as described in the skill instructions.
- Tailwind needs to be compiled during development. Compile it before delivery so the final HTML opens without Node.js, a CDN, or a runtime build.

## Feedback, maintenance, and licensing

Read [CONTRIBUTING.md](CONTRIBUTING.md) before submitting improvements. See [CHANGELOG.md](CHANGELOG.md) for version history and [SECURITY.md](SECURITY.md) for sensitive issues. Report reproducible problems through [GitHub Issues](https://github.com/ducafecat/design-ui-ux/issues).

The project does not yet have a license. Check the relevant permissions before using or redistributing it. Before publishing, the maintainer needs to verify the sources, redistribution rights, and licenses for the code and data. A listed source does not, by itself, grant permission to redistribute. See the [source notice](NOTICE.md).
