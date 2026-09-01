# AGENTS.md

## Project
A beginner-level static website built as part of a coding bootcamp course
("DevBootcamp"). It is a plain HTML/CSS project — no build tools, bundlers,
package manager, or JavaScript framework. There is no `package.json`.

- [index.html](index.html) — the single page of the site.
- [styles.css](styles.css) — all styling, linked from `index.html`.

Preview changes by opening `index.html` directly in a browser (or use a
"Live Server"-style extension) — there is no dev server or build step.

## Conventions
- Theme colors are defined once as CSS custom properties in the `:root`
  block at the top of [styles.css](styles.css#L3) (e.g. `--color-navy`,
  `--color-purple`, `--gradient-hero`). Always reuse these variables for
  new styles instead of hardcoding hex colors, so the palette stays
  consistent.
- Layout is done with Flexbox (see `.site-header`, `.site-nav ul` in
  [styles.css](styles.css)) rather than CSS Grid or floats.
- Keep HTML semantic (`<header>`, `<nav>`, `<ul>`) rather than generic
  `<div>` soup.

## Audience
This repo is for learning. When making changes, prefer small, easy-to-follow
edits and simple, well-explained CSS/HTML over advanced or clever patterns.
