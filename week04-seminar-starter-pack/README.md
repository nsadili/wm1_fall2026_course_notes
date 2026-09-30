# Week 4 Seminar Responsive Vehicle Listings

## Goal

Transform the supplied semantic HTML into a responsive vehicle-listing page. The cards must show one item per row on small screens, two on tablet-sized screens and four on desktop screens. Use Flexbox as the main layout method.

Do not modify the listing information unless an instruction explicitly requires an HTML change. Font Awesome is installed locally and already connected in `index.html`. `variables-example.css` contains one small example of declaring a reusable value in `:root` and using it on `body`. Write the remaining CSS in `styles.css`.

## Before you begin

1. Open `index.html` in a browser.
2. Open Developer Tools and inspect the page in normal flow.
3. Resize the viewport and observe that no responsive card layout exists yet.
4. Locate `.card-list`, `.car-card`, `.car-card__image`, `.favorite`, `.promo-badges` and `.status-tags` in the HTML.

## Task 1 Apply foundational rules

1. Set `box-sizing: border-box` for all elements.
2. Remove the default body margin and choose a readable system font.
3. Make images block-level and limit their maximum width to `100%`.
4. Create a centred `.container` with a maximum width and responsive side spacing.
5. Add reusable custom properties in `:root` for the surface, text, muted text, accent, border and card radius.

## Task 2 Arrange the header with Flexbox

1. Make `.header-inner` a flex container.
2. Align its direct children vertically.
3. Place available space between the brand, navigation and button.
4. Add `gap` and allow wrapping so the header does not overflow.
5. Remove the list markers and padding from `.nav-list`, then arrange its links with Flexbox.

## Task 3 Create the mobile card layout

1. Make `.card-list` a flex container.
2. Enable wrapping with `flex-wrap: wrap`.
3. Add consistent spacing using `gap`, not a right margin on every card.
4. Make every `.car-card` occupy one full row by default.
5. Style the cards with a white surface, border, rounded corners and hidden overflow.
6. Give each image wrapper a consistent aspect ratio and use `object-fit: cover` on its image.

Expected result: at narrow widths, all ten cards form one vertical column.

## Task 4 Position the controls and labels

1. Make `.car-card__image` the positioning reference using `position: relative`.
2. Position `.favorite` in the top-right corner.
3. Position `.promo-badges` in the top-left corner.
4. Arrange simultaneous Premium and VIP badges horizontally using Flexbox and `gap`.
5. Position `.status-tags` near the bottom-left of the image.
6. Let status tags wrap when several tags appear on one card.
7. Give each status type a distinguishable colour.

Do not absolutely position the complete card. Only the overlay controls and labels should leave normal flow.

## Task 5 Add the tablet breakpoint

At `40rem` or another justified width where space permits, change each card to:

```css
flex-basis: calc((100% - 1rem) / 2);
```

The subtraction accounts for one gap between two cards.

Expected result: two cards per row.

## Task 6 Add the desktop breakpoint

At `64rem` or another justified desktop width, change each card to:

```css
flex-basis: calc((100% - 3rem) / 4);
```

Four cards create three gaps. Use `flex-grow: 0` so the final two cards retain the same width rather than expanding across the final row.

Expected result: four cards per row, producing rows of four, four and two.

## Task 7 Refine the visual design

1. Style the price as the strongest text in each card.
2. Keep secondary location and time information visually quieter.
3. Provide visible hover feedback for the favourite and new-listing buttons.
4. Check text contrast and keep icon buttons keyboard-accessible.
5. Ensure long model names do not force the cards to overflow.

## Task 8 Test the result

1. Test a narrow mobile viewport.
2. Test immediately below and above `40rem`.
3. Test the widths between tablet and desktop.
4. Test immediately below and above `64rem`.
5. Continue dragging the viewport rather than checking only preset devices.
6. Confirm that cards never overlap and that badges remain attached to their own image.

## Completion checklist

- [ ] One card per row on mobile
- [ ] Two cards per row on tablet
- [ ] Four cards per row on desktop
- [ ] Ten cards remain visible at every width
- [ ] Last desktop row does not stretch its two cards
- [ ] Heart is positioned at the top-right of every image
- [ ] Premium and VIP can appear together
- [ ] Image tags can wrap when several are present
- [ ] Layout uses Flexbox rather than Grid
- [ ] No horizontal page scrolling

## Finish early

Choose one extension:

1. Add a hover state that fills the heart icon without JavaScript.
2. Add a fourth breakpoint only if you can demonstrate a real layout failure that requires it.
3. Add one more listing card and explain how it changes the final desktop row.
4. Use a custom property to change every card radius from one place.

## Submission

Submit the project folder with `index.html`, `variables-example.css` and your completed `styles.css`. Include one desktop screenshot and one mobile screenshot.
