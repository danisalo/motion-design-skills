# Accessible equivalents and control

## Reduced motion

Define the equivalent per component before implementation. Preserve the information and function rather than a specific effect. Replace large travel, zoom, parallax, and oscillation with immediate state or a short opacity change where appropriate. Provide a stable label/icon for success, error, and waiting; a rotating spinner is not automatically essential.

Keep default content readable during setup, server rendering, and script failure. For elaborate effects, opt into movement when the preference permits it. Apply the preference to CSS, JavaScript timelines, canvas, native animation, and live preference changes. Inspect the chosen framework's behavior rather than assuming one CSS query controls every mechanism.

Prefer targeted alternatives. A global near-zero duration reset is only a backstop and may leave loops/event-dependent state incorrect. Keep semantic state independent of decorative transition-end events.

## Distinct accessibility checks

| Check | Conditions and action |
|---|---|
| WCAG 2.3.3, AAA | Allow interaction-triggered motion animation to be disabled unless essential to function/information |
| WCAG 2.2.2, A — movement | For automatically starting moving/blinking/scrolling information lasting >5s alongside other content, provide pause/stop/hide unless the activity is essential |
| WCAG 2.2.2, A — updates | Provide control over automatic updating alongside other content unless essential; this clause has no five-second threshold |
| WCAG 4.1.3, AA | Make displayed status messages programmatically identifiable so assistive technology can present them without moving focus |
| WCAG 2.5.7, AA | Provide a single-pointer alternative to author-defined dragging unless an exception applies; keyboard support is separate |

Apply the levels and conditions accurately. This checklist does not establish complete WCAG conformance. Check flashing against current applicable W3C guidance if an effect flashes; prefer a stable signal that avoids the issue.

## Interaction semantics

Preserve focus visibility, component roles, expanded/selected state, and the appropriate focus-entry/return behavior. Make pointer targets usable throughout permitted transitions. Express errors with readable descriptions and correction paths; avoid relying on shaking or color alone. Expose important status without unnecessary repeated live announcements.

Offer click/tap alternatives to drag where required, as well as keyboard operation. Use hover as enhancement; retain the affordance on touch and keyboard. Allow cancel/reverse when the interaction permits it. Keep critical content accessible when a timeline is paused or removed.

## Verification

Exercise normal and reduced motion; changes to the preference where supported; keyboard/touch/pointer; focus while opening/closing; and static/setup-failure states. Confirm information remains equivalent, not merely that transforms disappear. Mark inaccessible device or assistive-technology checks as unverified.
