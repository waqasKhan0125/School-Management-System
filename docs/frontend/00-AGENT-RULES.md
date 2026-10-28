# Strict Rules for the Coding Agent

## Implementation phase
- **Phase:** Phase 0 — Read and confirm; applies to every phase
- **Before starting:** Follow the mandatory phase gates and reference-image rules throughout implementation.
- **Required workflow:** Read this file fully, inspect existing files, tell the user what will change, implement only this phase, test, compare with the reference image where relevant, and report results. Do not move to the next phase without review.


## Non-negotiable visual rule
The provided images are the required target, not loose inspiration. Do not redesign, modernize, simplify, recolor, rearrange, or replace their composition with a generic admin template. Keep the same visual hierarchy, placement, proportions, whitespace, colors, rounded corners, gradients, and overall look as closely as practical.

### Required workflow
1. Read this file and all relevant page specs before coding.
2. Inspect the actual repository and `apps/web` structure. Report what exists before making assumptions.
3. Use the supplied images in `reference-images/` for visual comparison.
4. Implement shared design tokens and reusable components before individual pages.
5. Match the screenshot at its reference canvas ratio first, then make it responsive.
6. Capture/inspect the page after implementation and fix obvious mismatches before moving on.
7. Use real app data when available. If backend data is not ready, use clearly named mock data in a separate mock-data module; never present example figures as live database results.

## Do not do these things
- Do not invent a new design.
- Do not change the sidebar from the left to the top on desktop.
- Do not replace the navy + green/teal palette with purple, blue-only, black-only, or another theme.
- Do not make the design cyberpunk, glassmorphism-heavy, or overly animated.
- Do not add Google or Microsoft sign-in. SchoolFlow is an offline-first single-school desktop application.
- Do not add in-app notifications or an events module merely because the reference screenshot contains sample events.
- Do not hard-code sample names, dates, student totals, attendance percentages, or class counts as real values.
- Do not place the entire app in one giant file. Use small, understandable components and page files.
- Do not add dependencies without checking whether the current project already has an equivalent.
- Do not change API/database/desktop implementation while doing frontend-only work unless explicitly asked.

## Adaptation policy
Only product-specific elements may change where required: sample user name/data, role-specific menu items, actual SchoolFlow module names, offline authentication, and language selector. These changes must preserve the reference's visual style and layout. If a requirement conflicts with the reference's decorative example content, functionality wins but visual composition should remain similar.

## Explain your work
For each phase, tell the student in simple English what files were created/changed and why. Keep a short list of remaining tasks. Do not claim a page is complete unless it has been checked against its specification.


## Mandatory phased workflow
1. Read the root `PHASE-PLAN.md` and follow its sequence.
2. Do not write code during Phase 0. First explain the plan and wait for user approval.
3. Work on one phase at a time; do not generate the whole frontend in one response.
4. Before each phase, list exact files to create/change. Afterward, list files changed, checks run, and anything not yet verified.
5. Stop at each phase gate for user review.
6. The two supplied reference images are the visual source of truth. Do not change their composition, layout, proportions, card arrangement, sidebar placement, or palette without explicit approval.


## Important: phases must be inside each page file
Follow the phases written inside the selected page specification. Example: `02-LOGIN-PAGE.md` has Phase 1 for the left branding panel, Phase 2 for the right login card, Phase 3 to assemble them, then responsive, functional, and visual-review phases. Apply the same page-by-page phased approach to dashboards and modules. Do only the current phase, check it, and report before proceeding.
