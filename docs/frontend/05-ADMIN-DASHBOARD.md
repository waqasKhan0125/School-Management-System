# Admin/Clerk Dashboard

Use the same shell, sidebar style, typography, spacing, cards and header structure as the Principal dashboard reference. Do not invent a different theme.

## Content
- Student totals and admission shortcut only if permitted.
- Today's attendance overview and shortcut only if permitted.
- Fee collection / outstanding summary only if fee permissions are granted.
- Class overview and frequently used tasks based on granted permissions.

## Access rules
Admin and Clerk are one combined role in this project, not two separate roles. Principal configures View/Create/Edit/Delete/Print-Export permissions per module. Hide unavailable navigation items and block direct route access when unauthorized. Do not show Settings, Users & Permissions, Audit Log or unrestricted backup restore by default. Apply the precise permissions from the authorization layer when implemented.
