# Login Page Specification

## Required visual target
Follow `reference-images/01-login-reference.jpg `. Do not substitute a standard centered login box. Desktop must show the large light outer frame, dark left branding panel and white right login card in the same composition.

## Left branding panel
Order and alignment:
1. SchoolFlow school/building logo centered near the top.
2. `SCHOOLFLOW` brand name below the logo, uppercase and bold.
3. Small mint/teal pill: `EDU • v2.1` (version text should come from app configuration later; do not hard-code a misleading release version).
4. Large school/building illustration centered in the middle.
5. `Welcome to` and large `SCHOOLFLOW` near the lower-middle area.
6. `School Management System` with thin decorative horizontal lines on either side.
7. Small footer tagline: `Empowering schools • Secure • Reliable • Scalable`.
8. Navy background with subtle teal glow, soft blur lights and a few small green/teal dots, matching screenshot placement. Keep effects restrained.

## Right login area
- White rounded card with subtle shadow, centered in the right area.
- Heading: `Welcome back`.
- Subtitle: `Sign in to your account`.
- Username/email field with envelope icon and placeholder `you@gmail.com` unless the final authentication spec chooses username instead. Do not add both username and email without a requirements decision.
- Password field with lock icon, masked by default, eye toggle on the right.
- One row: `Remember me` checkbox on left; `Forgot password?` link on right.
- Wide primary `Sign In` button with green-to-teal horizontal gradient.
- Below the card/form area: lock icon and `All data secure & encrypted` note.

## Product-specific differences from the screenshot
- Remove Google and Microsoft sign-in buttons.
- Remove the `OR` divider that exists only to separate third-party sign-in.
- Keep local/offline authentication; do not make internet connectivity a condition for login.
- Provide English/Urdu language choice in a compact, unobtrusive place consistent with the visual style. Login language selection must not distort the main two-panel composition. Urdu mode must support RTL.
- No in-app notifications.

## Behavior
- Submit using Enter or the Sign In button.
- Disable the submit button while authentication is in progress and prevent duplicate submissions.
- Show a concise, safe error message on failed login; do not reveal whether a particular username exists.
- Enforce the configured temporary lockout after five failed attempts; show a clear lockout message without exposing technical internals.
- Password visibility toggle changes only masking, not the password value.
- Forgot password must lead to the approved offline recovery flow; do not implement email reset or external identity-provider reset.
- Remember-me behavior must be limited to a safe remembered account/session preference; never store a plain-text password.
- Show loading, validation and failure states without changing the page composition.

## Acceptance criteria
- At desktop size, panel placement, proportions, colors, logo/illustration positions, heading hierarchy, input dimensions and gradient action closely match the supplied screenshot.
- No Google/Microsoft buttons or OR divider.
- Works with keyboard and screen readers.
- Responsive on small screens while retaining the same visual identity.
