# Shared App Layout

## Implementation phase
- **Phase:** Phase 1 — Shared visual foundation
- **Before starting:** Build and review the shared shell before role dashboards.
- **Required workflow:** Read this file fully, inspect existing files, tell the user what will change, implement only this phase, test, compare with the reference image where relevant, and report results. Do not move to the next phase without review.


## Desktop shell
Follow the dashboard reference image. The app shell has a dark navy vertical sidebar on the left and a large off-white/light main area on the right. Do not move the desktop navigation to the top.

### Sidebar anatomy
1. SchoolFlow logo and wordmark at the top.
2. Small `EDU • v2.1` badge below the wordmark.
3. Thin divider.
4. Vertical navigation list with line icons and labels.
5. Active route uses a rounded green-to-teal pill; inactive routes use muted gray/light text.
6. Current user avatar/initials, display name and role at the bottom, with a sign-out control.

### Main content area
- Large page heading at top left.
- Supporting description/greeting/date below it where appropriate.
- Page-level actions at top right.
- Consistent content padding and card grid.
- White cards with subtle shadow and rounded corners.
- Use the same icon style and spacing across all pages.

## Role navigation
- Principal: Dashboard, Students, Classes, Staff, Attendance, Exams & Results, Fees, Reports, Users & Permissions, Backup & Restore, Audit Log, Settings.
- Admin/Clerk: only modules/actions explicitly permitted by Principal; do not show Settings or Audit Log access by default.
- Teacher: Dashboard, assigned/authorized Students/Class information, Attendance, Exams & Marks, Results as permitted. Do not show fees, users, backup or settings unless a future approved permission explicitly allows them.
- Sidebar visibility must be derived from role/permissions, not just CSS hiding. Backend authorization will also be required later.

## Reusable components to implement
Use the repository's conventions if present. Suggested components:
- `AppShell`
- `Sidebar`
- `SidebarNavItem`
- `PageHeader`
- `PrimaryButton` / `SecondaryButton`
- `StatCard`
- `ContentCard`
- `SearchField`
- `DataTable`
- `StatusBadge`
- `ConfirmDialog`
- `EmptyState`
- `LoadingState`
- `ErrorState`
- `LanguageSwitcher`

Avoid giant files. Keep each component understandable and reusable.

## Responsive behavior
Desktop: full left sidebar. Tablet: compact sidebar/drawer if required. Mobile: drawer opened by a menu button, with the same navy/green visual style. Main content cards stack vertically at narrow widths.


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
