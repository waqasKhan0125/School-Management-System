# Admin/Clerk Dashboard

## Implementation phase
- **Phase:** Phase 3 — Role dashboards
- **Before starting:** Reuse approved shared components; show only Admin/Clerk permitted navigation/actions.
- **Required workflow:** Read this file fully, inspect existing files, tell the user what will change, implement only this phase, test, compare with the reference image where relevant, and report results. Do not move to the next phase without review.


Use the same shell, sidebar style, typography, spacing, cards and header structure as the Principal dashboard reference. Do not invent a different theme.

## Content
- Student totals and admission shortcut only if permitted.
- Today's attendance overview and shortcut only if permitted.
- Fee collection / outstanding summary only if fee permissions are granted.
- Class overview and frequently used tasks based on granted permissions.

## Access rules
Admin and Clerk are one combined role in this project, not two separate roles. Principal configures View/Create/Edit/Delete/Print-Export permissions per module. Hide unavailable navigation items and block direct route access when unauthorized. Do not show Settings, Users & Permissions, Audit Log or unrestricted backup restore by default. Apply the precise permissions from the authorization layer when implemented.


## In-file implementation phases

Complete this file in the phases below. These phases belong to THIS file; do not rely only on the global plan.

### Phase 1 — Structure and reference layout
Create only the main page regions. Match the relevant supplied reference's layout, proportions, spacing, background, and alignment. Do not invent widgets or redesign the page.
**Check:** compare the running page with the reference before proceeding.

### Phase 2 — Shared visual components
Apply the design-system colors, typography, sidebar/header rules, cards, buttons, fields, icons, borders, and spacing. Reuse shared components.
**Check:** sizes, colors, spacing, and alignment are consistent.

### Phase 3 — Page-specific content
Implement the sections, tables, forms, summaries, and actions specified earlier in this file. Do not treat sample values in images as real production data.
**Check:** all required sections appear in the documented order.

### Phase 4 — Interactions, permissions, and states
Implement the required actions, search/filter behaviour, validation, loading/empty/error states, and role permissions. Keep offline-first requirements.
**Check:** controls work as labelled and unauthorized actions are blocked.

### Phase 5 — Responsive behaviour and accessibility
Preserve the approved desktop design while adapting smaller widths. Prevent clipping and horizontal scrolling; support keyboard focus and readable contrast.
**Check:** test laptop/desktop and narrow widths.

### Phase 6 — Visual and functional review
Compare the running page to the reference and this file's requirements. Fix differences, test visible controls, and report completed phases and changed files.
**Check:** do not claim completion while required checks fail.
