# Shared App Layout

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
