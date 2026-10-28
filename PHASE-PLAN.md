# SchoolFlow Frontend — Implementation Phase Plan

This plan is mandatory for both the student and the coding agent. Follow the phases in order. Do not skip ahead or implement all pages in one large generation.

## Phase 0 — Read and confirm (no coding)
**Read:** `START-HERE.md`, `docs/frontend/README.md`, `00-AGENT-RULES.md`, both reference images, and `01-DESIGN-SYSTEM.md`.
**Agent deliverable:** explain the existing repository, list the proposed files to create, identify uncertainties, and confirm the reference-image layout. Do not write code until this review is complete.
**Gate:** user reviews and approves the plan.

## Phase 1 — Shared visual foundation
**Files:** `01-DESIGN-SYSTEM.md`, `03-SHARED-APP-LAYOUT.md`.
**Implement:** design tokens, typography, reusable buttons/inputs/cards, app shell, fixed desktop sidebar, active menu treatment, page container, responsive behavior.
**Gate:** compare a shell preview with the dashboard reference before proceeding. Do not invent new styling.

## Phase 2 — Login page
**File:** `02-LOGIN-PAGE.md`.
**Implement:** two-panel layout matching the supplied login image, branding panel, logo/illustration placement, login form, password visibility, validation and language selection. Do not include Google/Microsoft login or in-app notifications.
**Gate:** compare screenshot at the same desktop aspect ratio; correct layout differences before moving on.

## Phase 3 — Role dashboards
**Files:** `04-PRINCIPAL-DASHBOARD.md`, `05-ADMIN-DASHBOARD.md`, `06-TEACHER-DASHBOARD.md`.
**Implement:** shared shell with role-specific navigation, permitted actions, dashboard summaries and genuine data/loading/empty/error states. Use sample data only when clearly marked as demo.
**Gate:** verify each role sees only authorized modules/actions.

## Phase 4 — Main modules
**Files, in order:**
1. `07-STUDENT-PAGES.md`
2. `08-STAFF-PAGES.md`
3. `09-ATTENDANCE-PAGES.md`
4. `10-EXAMS-RESULTS-PAGES.md`
5. `11-FEES-PAGES.md`
6. `12-REPORTS-PAGES.md`

Implement one module at a time. Reuse the design system and shared components. For each module, finish listing/table, search/filter, form/detail views, validation, permission states, and loading/empty/error states before starting the next module.
**Gate:** run the relevant checklist and show the user what changed.

## Phase 5 — Responsive and visual QA
**File:** `13-IMPLEMENTATION-CHECKLIST.md`.
Test the desktop reference match, narrower laptop widths, keyboard focus, forms, navigation, role permissions, English/Urdu layout including RTL, and all visible states. Fix mismatches before calling the frontend complete.

## Required workflow for every phase
1. Read the corresponding MD file completely.
2. Inspect the current repository and reuse existing files where appropriate.
3. Tell the user which files will be created/changed and why.
4. Implement only the current phase.
5. Run available checks and report actual results; never claim unrun tests passed.
6. Compare the result against the supplied images where relevant.
7. Ask for user review at the phase gate before proceeding.

## Important boundary
This pack is a specification, not finished application code. Backend/database work is out of scope during these frontend phases. Do not fabricate exact features or redesign the supplied reference. If a requirement conflicts with the offline SchoolFlow requirements, flag it and ask instead of silently guessing.
