# Exams and Results Pages

## Implementation phase
- **Phase:** Phase 4 — Main modules, item 4
- **Before starting:** Start after Attendance pages pass review; follow configurable exam and publication requirements.
- **Required workflow:** Read this file fully, inspect existing files, tell the user what will change, implement only this phase, test, compare with the reference image where relevant, and report results. Do not move to the next phase without review.


## Exams
- Exam list and exam-type management for authorized users.
- Principal configures exam types, grading boundaries and pass percentage.
- Exam form includes name/type, academic period, classes and subjects as configured.

## Marks entry
- Subject-wise obtained marks and total marks.
- Validate that values are numeric, non-negative and do not exceed total marks.
- Teachers can enter marks only for authorized classes/subjects.
- Provide save state and prevent accidental navigation with unsaved changes when feasible.

## Results
- Permitted teacher may publish results directly, according to the approved project requirement.
- Display result status clearly (draft/published if those states are implemented).
- Report card includes school logo, student details/photo if available, marks, grades, attendance, remarks and promotion status.
- Promotion is manually selected and requires Principal confirmation; a failed student may remain in the same class.

Keep all pages visually aligned with the supplied dashboard reference. Avoid fake charts or fabricated marks.


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
