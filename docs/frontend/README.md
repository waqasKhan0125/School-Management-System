# SchoolFlow Frontend — Exact Reference Pack

## Implementation phase
- **Phase:** Phase 0 — Read and confirm
- **Before starting:** Explain the frontend documentation and phase sequence to the user before coding.
- **Required workflow:** Read this file fully, inspect existing files, tell the user what will change, implement only this phase, test, compare with the reference image where relevant, and report results. Do not move to the next phase without review.


## Purpose
This folder is the frontend design and implementation specification for SchoolFlow. It is written for both the student developer and the coding agent. The two images in `reference-images/` are the visual source of truth.

## Start here
1. Read `00-AGENT-RULES.md` first.
2. Open both reference images at full size.
3. Read `01-DESIGN-SYSTEM.md` and `02-LOGIN-PAGE.md`.
4. Implement the shared layout and login first. Then build each page using the same visual system.
5. After each page, compare a screenshot of the implementation against the reference before continuing.

## Files
- `reference-images/01-login-reference.jpg`: supplied login screen.
- `reference-images/02-dashboard-reference.jpg`: supplied dashboard screen.
- `00-AGENT-RULES.md`: strict implementation instructions; prevents redesign.
- `01-DESIGN-SYSTEM.md`: visual tokens and layout measurements.
- `02-LOGIN-PAGE.md`: login page specification.
- `03-SHARED-APP-LAYOUT.md`: sidebar, page header, content area and responsive behavior.
- `04-PRINCIPAL-DASHBOARD.md`: dashboard structure and real-data requirements.
- `05-ADMIN-DASHBOARD.md`: Admin/Clerk dashboard.
- `06-TEACHER-DASHBOARD.md`: Teacher dashboard.
- `07-STUDENT-PAGES.md`: student list and admission form.
- `08-STAFF-PAGES.md`: staff pages.
- `09-ATTENDANCE-PAGES.md`: attendance pages.
- `10-EXAMS-RESULTS-PAGES.md`: exam and results pages.
- `11-FEES-PAGES.md`: fee pages.
- `12-REPORTS-PAGES.md`: report pages.
- `13-IMPLEMENTATION-CHECKLIST.md`: acceptance checklist.

## Important scope boundary
These are frontend specifications, not a claim that the app is already implemented. Do not create backend/database features in this task. The app's existing monorepo structure should be inspected before creating source files. If source files are empty, build them cleanly; do not assume existing components are present.


## How to use the phases
Each page specification contains its own implementation phases. For example, `02-LOGIN-PAGE.md` begins with Phase 1 (left branding panel only), then Phase 2 (right login form), Phase 3 (assemble full screen), followed by responsive behaviour, functionality, and visual review. Follow phases within each file in order.
