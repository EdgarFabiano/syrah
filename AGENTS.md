# AGENTS.md - Syrah Centro Clínico

## Project Overview

Static single-page website for a medical clinic built with plain HTML, CSS, and JavaScript (no frameworks). The entire site is contained in `index.html`.

---

## Build & Development Commands

Since this is a plain static HTML project, there is no build system required.

- **Preview**: Open `index.html` directly in a browser, or use a local server:
  ```bash
  # Python
  python -m http.server 8000
  # Node
  npx serve .
  ```
- **Linting**: No automated linting configured. Manual review follows the style guidelines below.
- **Testing**: No automated tests. Browser testing should verify:
  - Responsive layout at mobile/tablet/desktop breakpoints
  - Smooth scrolling and navigation
  - WhatsApp links open correctly
  - Insurance filter functionality works
  - Animations render without jank

---

## Code Style Guidelines

### General Principles

- Keep HTML semantic and accessible
- Use CSS custom properties (variables) for colors and spacing
- Write vanilla JavaScript without dependencies
- Ensure responsive design works across breakpoints (768px, 1024px)

### HTML

- Use semantic elements: `<header>`, `<nav>`, `<section>`, `<main>`, `<footer>`
- Include proper meta tags for SEO and accessibility
- Use `lang="pt-BR"` for Portuguese content
- Alt text for all images (use descriptive placeholders if images are missing)
- Keep attribute order consistent: `class`, `id`, `src`, `alt`, `href`, `type`

### CSS

- Use CSS custom properties for all colors (see existing `:root` pattern)
- Follow the pattern: `--primary`, `--primary-dark`, `--primary-light`, `--gold`, etc.
- Use flexbox and grid for layout; avoid floats
- Preferrem (rem) over px for font sizes and spacing
- Use BEM-like naming for component classes (e.g., `.header__inner`, `.logo-icon`)
- Mobile-first approach: base styles for mobile, `@media (min-width)` for larger screens
- Group related styles together (layout, typography, components, utilities)
- Use consistent indentation (4 spaces)

### JavaScript

- Use `const` and `let`; avoid `var`
- Use strict equality (`===` over `==`)
- Prefer ES6+ syntax: arrow functions, template literals, destructuring
- Wrap IIFE or use modules if adding new scripts
- Add event listeners with `{ passive: true }` for scroll/pointer events
- Handle edge cases (null checks for `document.querySelector`)
- Add comments for complex logic (e.g., insurance filter, scroll observer)

### Naming Conventions

- **Classes**: lowercase with dashes (e.g., `.fade-in`, `.insurance-grid`)
- **Variables**: camelCase (e.g., `visibleCount`, `currentScroll`)
- **Functions**: camelCase, descriptive names (e.g., `filterInsurance`, `toggleInsurance`)
- **Constants**: SCREAMING_SNAKE_CASE if truly constant (e.g., `observerOptions`)

### Accessibility

- Ensure keyboard navigation works (tab order, focus states)
- Use sufficient color contrast (verify gold accents are readable)
- ARIA labels for interactive elements without text
- Form inputs should have associated `<label>` elements

### Error Handling

- JavaScript: wrap DOM queries in null checks
- Links to external resources (WhatsApp, Google Maps) should open in new tab
- Graceful degradation: site should work without JavaScript (core content visible)

---

## Project Structure

```
syrah/
├── index.html    # Complete single-page website (HTML + CSS + JS)
├── README.md     # Project documentation
├── SPEC.md       # Design specification
└── AGENTS.md     # This file
```

---

## Content Guidelines

- All content is in Brazilian Portuguese
- Use professional medical terminology
- Maintain consistent tone: welcoming, professional, trustworthy
- Contact info: (61) 99866-3538, WhatsApp link: https://wa.me/5561998663538

---

## Common Tasks

### Adding a new section
1. Add semantic `<section>` wrapper in HTML
2. Use existing container class for max-width
3. Follow color variables from `:root`
4. Add fade-in animation class for scroll effects

### Modifying colors
Edit CSS variables in the `:root` block at the top of `<style>`

### Adding JavaScript functionality
1. Add at the end of `<script>` tag before closing body
2. Wrap in DOMContentLoaded or place at end of body
3. Test in multiple browsers

---

## Brand Guidelines (Reference)

- **Primary**: #1f4d2b (Deep Green)
- **Gold Accent**: #c9a227
- **Font**: DM Sans (Google Fonts)
- **Target audience**: Patients seeking nutrition, wellness, and medical care in Brasília/Águas Claras