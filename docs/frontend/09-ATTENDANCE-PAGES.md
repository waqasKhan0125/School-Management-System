# Attendance Pages

## Implementation phase
- **Phase:** Phase 4 — Main modules, item 3
- **Before starting:** Start after Staff pages pass review; enforce authorized attendance correction rules.
- **Required workflow:** Read this file fully, inspect existing files, tell the user what will change, implement only this phase, test, compare with the reference image where relevant, and report results. Do not move to the next phase without review.


## Visual layout
Shared app shell; page title and date/class filters above a white table/card. Use clear status pills consistent with the green/teal palette and readable neutral styles for other states.

## Features
- Daily attendance statuses: Present, Absent, Leave, Late.
- Select class/section and date, then show the authorized student list.
- Provide clear bulk marking where allowed and a visible save action.
- Show summary counts without hard-coded numbers.
- Teacher can mark attendance for any class only when permitted.
- Only Principal/Admin may correct already saved attendance, subject to permissions.
- Confirmation and audit trail are required for corrections.
- Do not imply that a change is saved until the save operation succeeds.

Provide no-record, loading, save-success and safe error states. Support keyboard use and readable status labels; do not rely on color alone.


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
