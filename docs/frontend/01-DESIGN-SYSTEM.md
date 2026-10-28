# Design System — Match the Supplied Images

## Implementation phase
- **Phase:** Phase 1 — Shared visual foundation
- **Before starting:** Complete design tokens and reusable styles first. Validate the app shell against the supplied dashboard image.
- **Required workflow:** Read this file fully, inspect existing files, tell the user what will change, implement only this phase, test, compare with the reference image where relevant, and report results. Do not move to the next phase without review.


## Source of truth
- Login: `reference-images/01-login-reference.jpg` (1920 × 1280 source image; visible composition has a light outer canvas, a large rounded white application frame, a dark navy branding panel on the left and login card on the right).
- Dashboard: `reference-images/02-dashboard-reference.jpg` (1920 × 1280 source image; left vertical navy sidebar and large light main workspace).

Treat the screenshots as visual references. Exact source-image pixels may be sampled during implementation; do not approximate by choosing an unrelated theme.

## Palette
Use CSS custom properties so colors can be tuned centrally against the images:
- `--sf-navy`: deep near-black navy for branding panel/sidebar (reference approximately `#07152D` to `#0B1831`).
- `--sf-navy-soft`: slightly lighter navy/blue-green blend for panel depth.
- `--sf-green`: bright mint/green used at the start of gradients and positive accents (approximately `#43D38B`).
- `--sf-teal`: teal used at the end of gradients and active accents (approximately `#078A98`).
- `--sf-green-dark`: muted green for labels and secure-status text (approximately `#287A68`).
- `--sf-page`: very light neutral/off-white page background (approximately `#F7F8FA`).
- `--sf-surface`: white card surface (`#FFFFFF`).
- `--sf-text`: dark navy primary text (approximately `#111D35`).
- `--sf-muted`: gray secondary text (approximately `#777B82`).
- `--sf-border`: light gray borders (approximately `#D5D7DB`).

These hex values are starting estimates from the visible reference, not permission to change the palette. Fine-tune against the actual images.

## Typography
- Use a clean sans-serif similar to the reference; prefer the existing project font if one is already configured. Otherwise use `Inter` or a close system sans-serif. Avoid decorative fonts.
- Primary text is dark navy/black; supporting text is medium gray.
- The login headline is large and bold; form labels are clear and medium-weight.
- Dashboard page title is very large and bold on desktop, with a smaller greeting/date line beneath it.
- Avoid tiny text. Preserve the hierarchy shown in the screenshots.

## Shape, borders and depth
- Cards: white, rounded corners, subtle soft shadows, no heavy outlines.
- Inputs: pale gray-white fill, thin gray border, rounded corners, icon inside left edge; password visibility control at right.
- Primary action: horizontal mint-green-to-teal gradient, white bold text, rounded corners, subtle shadow.
- Sidebar: deep navy with gentle teal glow/gradient toward lower/right regions, rounded outer corners where the reference frame shows them.
- Active sidebar item: rounded pill with green-to-teal gradient; inactive items use muted light gray text and line icons.
- Decorative glow dots/blur on login branding panel should be subtle and positioned like the reference, not spread across all pages.

## Login layout rules
- On desktop, use the two-panel composition: branding panel on the left (about 45% of the inner app frame) and login area on the right (about 55%).
- Keep generous whitespace and the outer light background/frame.
- Branding panel has the logo and SCHOOLFLOW near the top, small `EDU • v2.1` badge, large school/building illustration in the middle, welcome title and subtitle lower down, and short tagline near the bottom.
- Login card is white, centered in the right region, with a large “Welcome back” title and subtitle, stacked inputs, remember/forgot row, wide gradient Sign In button, and secure-data note beneath.
- The reference image includes Google/Microsoft sign-in. Do NOT implement those buttons or the `OR` divider; offline-only product requirements override that part. Preserve the remaining alignment by using the available form space naturally; do not redesign the entire card.

## Dashboard layout rules
- Desktop sidebar stays on the LEFT and spans nearly the full application height.
- Main content occupies the remaining width with a light background.
- Header: large `Dashboard` title on left, greeting/date below; `Add Student` and `Export Report` actions on the right for roles permitted to use them.
- Main dashboard grid: two columns, two rows at the reference desktop size. Top-left student overview; top-right attendance rate; bottom-left classes overview; bottom-right upcoming-events area replaced by a relevant school summary (e.g., fee collection or exam summary) because SchoolFlow has no events module requirement. Keep card size, rounded edges and spacing consistent with screenshot.
- Keep the large values, small descriptions, colored chips and circular attendance visualization in the same visual hierarchy.
- Sidebar logo block at top; menu items vertically spaced; profile/avatar and role at the bottom.
- Footer is understated and contains product name, school management system, update/status text only if real and available.

## Responsive behavior
- Match desktop first at 1536 × 1024 and 1920 × 1280 proportions.
- At narrower widths, preserve the same colors, component shapes, hierarchy and order. Collapse the sidebar into a drawer or compact rail only when necessary; do not convert the desktop layout into a top navbar.
- At mobile widths, stack dashboard cards in one column and make form fields/buttons full width.
- Prevent horizontal overflow; preserve usable spacing and readable text.

## Interaction and accessibility
- Keyboard focus must be visible, but visually consistent with the green/teal palette.
- Inputs need associated labels; icon-only controls need accessible names.
- Buttons, links, menus and password visibility must work, not merely look clickable.
- Respect reduced-motion preference. Animations should be subtle; the reference is primarily a static UI.
