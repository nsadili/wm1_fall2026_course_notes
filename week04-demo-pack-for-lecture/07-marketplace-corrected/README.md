# Loop Market responsive layout

This completed teaching example uses only HTML and CSS. Open `index.html` directly in a browser; no installation or server is required.

## Responsive states

- Mobile (below 768 px): one product column, a right-side hamburger menu, visible profile avatar, and stacked advertising.
- Tablet (768–1199 px): two product columns; the advertisement becomes a horizontal block below the listings.
- Desktop (1200 px and above): three product columns and a sticky right sidebar.

The CSS is mobile-first. Its two media queries create three states. This keeps the breakpoint logic visible enough for classroom inspection.

## Useful DevTools demonstrations

1. Inspect the header and identify its flex container and flex items.
2. Open the mobile hamburger and inspect the CSS-only `details` and `summary` menu.
3. Inspect `.product-grid` and toggle its Grid overlay.
4. Disable `box-sizing: border-box` and observe sizing changes.
5. Change viewport width around 768 px and 1200 px.
6. Inspect `.ad-sidebar` to see how one element changes layout and position.
7. Toggle `display: grid`, `position: sticky`, gaps, padding, and widths.
8. Inspect inherited text properties and overridden declarations.

The advertisement is intentionally static and contains no link.
