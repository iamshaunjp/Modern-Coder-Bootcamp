# PixelForge

Single landing page for a retro gaming review site. Plain HTML and CSS only: [index.html](index.html) and [styles.css](styles.css). No build step, tests, or package manager.

## Conventions

- **No third-party libraries or frameworks** (no CSS frameworks, JS libraries, icon kits). The only external resource is the Google Fonts Inter import already in `styles.css`.
- **Semantic HTML first**: use `header`, `nav`, `main`, `section`, `article`, `footer`, `figure`, etc. Keep the markup clean and minimal; avoid wrapper `div`s.
- **Use classes sparingly.** Prefer element and structural selectors (e.g. `header nav a`, `main > section`). When a class is needed, name it for its meaning (`.featured`, `.rating`), never its appearance (`.red-text`, `.big`).
- **Theme**: retro/pixel-game look, dark theme. All colours must come from the `--color-*` variables in `:root` in `styles.css` (bg, surface, text, primary, secondary, accent, success, warning, danger, info). Do not hard-code hex values outside `:root`; add a new variable there if one is missing.
- Keep all styles in `styles.css`; no inline styles.

## Pitfalls

- `index.html` links the stylesheet with an absolute path (`/styles.css`), so open it through a local server rooted at the project folder, not via `file://`.
