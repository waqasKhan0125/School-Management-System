# Teacher Dashboard

## Implementation phase
- **Phase:** Phase 3 — Role dashboards
- **Before starting:** Reuse approved shared components; show only permitted teacher actions.
- **Required workflow:** Read this file fully, inspect existing files, tell the user what will change, implement only this phase, test, compare with the reference image where relevant, and report results. Do not move to the next phase without review.


Use the exact shared SchoolFlow visual language from the dashboard reference: navy left sidebar, white/light content surface, large page title, green/teal accents and rounded white cards.

## Suggested dashboard cards
- Classes/sections assigned to the teacher.
- Today's attendance tasks for authorized classes.
- Exams/marks tasks that are pending or available to the teacher.
- Recent results or class summaries only if permission and data support them.

## Permissions
A teacher may mark attendance and enter marks for any class only when permitted. Teachers must not see unauthorized classes, student records or reports. Results publication is allowed to a permitted teacher according to the project decision. Do not show fees, staff salary, users, backup, settings or audit log by default.

Use empty states when no class/task is assigned. Do not show fake event lists or fabricated statistics.


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
