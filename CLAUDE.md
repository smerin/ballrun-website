# Project Guidelines

## CSS/SCSS
- Use rems, not pixels
- Use existing SCSS variables from `src/styles/_variables.scss`
- Follow BEM-style class naming for structural elements (e.g., `.hero__content`)
- Use data attributes for styling variants and states instead of BEM modifier classes:
  - `data-variant` for color/style variants (e.g., `data-variant="charcoal"`)
  - `data-layout` for layout variations (e.g., `data-layout="image-left"`)
  - Boolean attributes use presence/absence (e.g., `data-has-background`)
- Prefer ARIA attributes over data attributes where semantically appropriate:
  - `aria-current="page"` for active navigation links
  - `aria-hidden` for show/hide states (e.g., mobile nav)
  - `aria-expanded` for expandable elements
  - `aria-pressed` for toggle buttons
- Use attribute selectors in SCSS: `&[data-variant="white"]`, `&[aria-current="page"]`
- Use scoped styles in Astro components
