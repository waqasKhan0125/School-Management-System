# Implementation and Visual QA Checklist

## Before coding
- [ ] Inspect repository and existing `apps/web` files.
- [ ] Read all relevant docs and open both reference images.
- [ ] Confirm existing framework/router/font/icon packages before adding dependencies.

## Visual match
- [ ] Login has the two-panel desktop composition from the supplied image.
- [ ] Branding panel uses navy background, green/teal glow, logo, badge, illustration, welcome text and bottom tagline in the same order.
- [ ] Login card keeps the same heading, subtitle, input sizes, remember/forgot row, wide gradient button and secure note.
- [ ] Google/Microsoft buttons and OR divider are absent for offline product requirements.
- [ ] Dashboard has the left navy sidebar and large light workspace.
- [ ] Dashboard heading/greeting/actions match reference placement.
- [ ] Four-card dashboard grid matches reference arrangement at desktop size.
- [ ] Cards have white surfaces, rounded corners and subtle shadows.
- [ ] Active navigation and primary actions use the green-to-teal gradient.
- [ ] The implementation screenshot has been compared against the references and visual mismatches fixed.

## Functionality and quality
- [ ] No giant single-file implementation.
- [ ] Shared layout/components are reused across pages.
- [ ] No fabricated values presented as live data.
- [ ] Role-based navigation and route protection are implemented consistently.
- [ ] Forms have labels and validation; buttons and links work.
- [ ] Loading, empty, error and success states are provided where needed.
- [ ] English/Urdu switching and RTL are planned into layout.
- [ ] Responsive behavior avoids horizontal overflow.
- [ ] Keyboard focus and accessible labels are present.
- [ ] No Google/Microsoft login or in-app notifications added.

## Completion report format
At the end of each coding phase, list: (1) files created/changed, (2) what was implemented, (3) what is not implemented yet, (4) visual comparison result, and (5) exact next step. Do not claim exact visual matching without checking the rendered page against the reference image.
