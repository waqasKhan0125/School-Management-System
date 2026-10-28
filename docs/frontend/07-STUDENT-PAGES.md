# Student Pages

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
