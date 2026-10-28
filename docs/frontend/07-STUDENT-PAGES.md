# Student Pages

## Implementation phase
- **Phase:** Phase 4 — Main modules, item 1
- **Before starting:** Finish student list, search/filter, admission form, validation and states before starting staff pages.
- **Required workflow:** Read this file fully, inspect existing files, tell the user what will change, implement only this phase, test, compare with the reference image where relevant, and report results. Do not move to the next phase without review.


All student pages use the shared app shell and reference design system. Keep the same navy sidebar, light workspace, page heading, white cards, search controls, rounded fields and green/teal actions.

## Student list
- Page title `Students`; short description.
- Search by name/admission number and useful filters such as class/status.
- Main white card containing a clear table: admission number, student name, class/section, status, and permitted actions.
- Primary `Add Student` action only for users with create permission.
- Loading, no-results, empty and error states.
- Pagination only if needed by actual data volume.

## Admission form
- Use a readable grouped form, not a long single row of fields.
- Include only required/approved student fields; optional photo upload can be offered.
- Manual admission number. Warn about duplicates and require authorized confirmation if the business rule allows proceeding.
- Validate essential fields and show field-level errors.
- Save/cancel actions follow the common button styles.

## Student detail/edit
- Show identity and class information in a clean header/card, followed by relevant tabs/sections only where useful: profile, attendance, results and fee history subject to permission.
- Deletion must show confirmation. Soft delete/restore rules apply; permanent deletion is Principal-only and requires a second explicit confirmation.
- Never allow UI visibility alone to be the security control.


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
