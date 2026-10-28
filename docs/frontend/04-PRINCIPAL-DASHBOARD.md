# Principal Dashboard

## Implementation phase
- **Phase:** Phase 3 — Role dashboards
- **Before starting:** Use the approved shared shell; implement Principal-specific access and summaries.
- **Required workflow:** Read this file fully, inspect existing files, tell the user what will change, implement only this phase, test, compare with the reference image where relevant, and report results. Do not move to the next phase without review.


## Visual layout
Match `reference-images/02-dashboard-reference.jpg`:
- Left navy sidebar.
- Large `Dashboard` title and a one-line greeting/date beneath.
- Top-right actions aligned horizontally where space allows.
- Four main cards in a two-column/two-row grid on desktop.
- Card 1 top-left: Students Overview with a large total, supporting caption, month comparison only if valid data exists, and school-level distribution chips if configured.
- Card 2 top-right: Attendance Rate with a prominent circular progress ring, percentage centered inside, present/absent count underneath, and comparison only if valid historical data exists.
- Card 3 bottom-left: Classes with a large active-class count and small class/level breakdown chips.
- Card 4 bottom-right: replace reference's `Upcoming Events` with a useful SchoolFlow summary such as Fee Collection or Exam/Results Overview. Do not create an events module just to copy sample content.

## Header actions
- `Add Student`: visible only if the Principal has create-student permission (Principal normally has it).
- `Export Report`: opens the report/export flow; do not make a fake download.

## Data rules
- Never hard-code the reference values `1,284`, `92%`, `1,180`, `104`, or `24` as live results.
- Show actual API/database values when available.
- While the backend is not implemented, use clearly isolated mock data and label the app as demo/development mode.
- Handle empty school data gracefully (e.g. zero students/classes, no attendance recorded).
- Date format should follow selected language/locale.

## Interactions
Cards may link to their relevant modules when user permission allows it. Charts must include readable text equivalents; color alone must not convey status. All action buttons must work or be clearly disabled with an explanation.


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
