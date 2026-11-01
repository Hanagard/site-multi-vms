# Repository map

Static, single-page site for Multi VMS. No build system, framework, package manager, or backend.

## Dependency map

```text
index.html
├── styles.css          layout, components, responsive rules, dark/light palettes
├── script.js           mobile menu, theme toggle + localStorage, footer year
└── assets/             product screenshots used by the page

multi-vms-site.zip      portable bundle of the page, styles, script, and assets
```

## Edit guide

- Page sections, links, text, comparison cards, and image references: `index.html`.
- Visual changes, breakpoints, theme-specific colors: `styles.css`.
- Small browser interactions only: `script.js`.
- Replace or add product screenshots in `assets/`; update their references and alt text in `index.html`.
- Rebuild `multi-vms-site.zip` after source or asset changes.

## Important behavior

- Dark mode is the default. The header switch changes the root `data-theme` and saves `multi-vms-theme` in localStorage.
- The site is published with GitHub Pages from the repository root on `main`.
- The edition comparison is based on the legacy Multi VMS comparison page; its source link and capacity caveats are in the page.

## Change impact

Most content and styling changes need only `index.html` or `styles.css`. Interactive behavior changes need `script.js`. Image changes need the asset plus its HTML reference. There are no imported JS modules or generated source files.

