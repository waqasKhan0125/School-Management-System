# Fees Pages

## Implementation phase
- **Phase:** Phase 4 — Main modules, item 5
- **Before starting:** Start after Exams/Results pass review; include payment, balance, receipt and approval states.
- **Required workflow:** Read this file fully, inspect existing files, tell the user what will change, implement only this phase, test, compare with the reference image where relevant, and report results. Do not move to the next phase without review.


Use the shared shell and common white card/table styles. Financial values should be aligned consistently and use clear labels.

## Fee structure and bills
- Class-wise fee structure, monthly fees and admission fees.
- Monthly bill generation is manual.
- Monthly due date is configured by Principal.
- Discounts and manually entered late fines are permission-based; do not add a separate scholarship/concession module.

## Payments
- Support full, partial and installment cash payments with remaining balance.
- Show arrears by month and combined outstanding total.
- Manual receipt number; duplicate warning and authorized confirmation rules apply.
- Receipt can be printed or exported as PDF.
- Payment corrections and refunds are permission-based; refunds require Principal approval and audit history.

## UI behavior
- Confirm before consequential actions.
- Show amount due, paid amount and balance separately.
- Do not mark payment successful until backend confirmation.
- Restrict fee data/actions based on role and permission. Principal and authorized Admin/Clerk manage fees.


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
