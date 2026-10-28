# Login Page — Phase-by-Phase Implementation Specification

**Purpose:** Follow this file in order. Each phase is a separate implementation checkpoint. Do not skip phases or invent a different design.

**Visual source of truth:** `reference-images/01-login-reference.jpg`. Use the supplied image while coding and match its composition, proportions, colors, spacing, typography, corners, shadows, and visual hierarchy as closely as practical.

## Phase 1 — Left Branding Panel ONLY

Build only the left side of the reference. Do not build the right-side form in this phase.

- Large dark-navy panel on the left, with rounded outer corners.
- SchoolFlow logo/icon near the top, centered.
- `SCHOOLFLOW` brand name and small rounded `EDU · v2.1` label.
- Large green/teal school-building illustration in the middle.
- Lower branding text: `Welcome to`, `SCHOOLFLOW`, and `School Management System`.
- Small footer: `Empowering schools · Secure · Reliable · Scalable`.
- Subtle teal/green glow dots or blurred light effects placed like the reference.
- Preserve the reference's alignment and spacing; do not substitute a generic template.

**Acceptance checks:** left panel visually resembles the reference; logo, illustration, and text are centered and spaced correctly; colors match the reference. No login form or social login buttons in this phase.

**STOP:** run and compare the left panel with the screenshot. Get approval before Phase 2.

## Phase 2 — Right Login Card and Form

Only after Phase 1 is approved, implement the right side.

- Light neutral background and a white rounded login card with subtle shadow.
- Heading `Welcome back`; subtitle `Sign in to your account`.
- Account identifier field styled like the reference (the screenshot label is `Email`; follow the approved product requirement if username is selected).
- Password field with lock icon and working show/hide control.
- `Remember me` only if approved for the offline application.
- `Forgot password?` connected to the agreed offline recovery flow when implemented.
- Wide green-to-teal `Sign In` button.
- Match reference form spacing, input heights, button size, typography, and alignment.
- Do NOT add Google or Microsoft sign-in. This product is offline-first and these options are not approved.
- Include `All data secure & encrypted` footer only if it accurately reflects the implemented security.

**Acceptance checks:** card size and placement match the screenshot; form fields align; social login is absent; no fake successful authentication.

**STOP:** compare the right side with the screenshot before continuing.

## Phase 3 — Assemble the Split-Screen Composition

- Combine the approved left panel and right card.
- Preserve the reference's proportions, vertical alignment, outer container, rounded corners, light background, and soft shadow.
- Avoid changing approved Phase 1 and Phase 2 elements.

**Acceptance checks:** full page resembles the supplied image; no overlap, clipping, or uneven alignment.

## Phase 4 — Responsive Behaviour

- Keep the desktop/laptop design as close to the reference as possible.
- At narrow widths, stack/adapt panels without horizontal scrolling.
- Keep logo, form, and buttons readable and inside the viewport.
- Do not use responsive behaviour as an excuse to redesign desktop.

## Phase 5 — Functional Behaviour and Validation

- Account identifier and password are required.
- Password visibility toggle works.
- Show safe validation/error messages without revealing whether an account exists.
- Prevent duplicate submissions; show loading and failure states.
- Use offline authentication; do not assume internet access.
- Connect password recovery to the agreed offline recovery process.
- Support selected English/Urdu language and RTL for Urdu.
- Do not expose stack traces or sensitive technical details.

## Phase 6 — Visual Comparison and Final Review

Compare the running page side-by-side with `reference-images/01-login-reference.jpg`. Check panel proportions, logo placement, illustration size, text, fields, button, whitespace, colors, corners, and shadows. Fix differences before marking the page complete. Report files changed and checks performed.

## Agent execution rules

1. Work on one phase at a time.
2. Before a phase, state the target and expected files to change.
3. After a phase, run/check the page and report its acceptance checks.
4. Do not start the next phase until the current phase has been reviewed.
5. Do not create unrelated pages while implementing login.
6. Never replace the supplied design with a generic login template.
