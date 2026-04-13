# Coding Conventions

## JavaScript
- **Variables**: Prefer `const` and `let`.
- **Data Format**: The static database is an array of objects structured as `[{tab, iconClass, badge, title, template, examples: [...]}]`.
- **DOM Manipulation**: Manual DOM updates using `innerHTML` or `document.createElement`.

## CSS
- **Variables**: Extensive use of CSS custom properties (`:root`) for colors (theming, dark mode) and typography.
- **Naming**: Minimal BEM-like structure (e.g., `card-header`, `icon-prod`).
- **Layout**: Uses CSS Flexbox and Grid (`card-grid`, `tab-row`) for responsive behavior.

## HTML
- **Semantic HTML**: Proper use of `<header>`, `<main>`, `<button>`, `<input>`.
- Inline onclick/oninput handlers for top-level interactive elements (search, tab buttons).
