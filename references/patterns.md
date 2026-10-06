# Behavior patterns

Choose a pattern only after the eligibility gate. Read the entry for the affected component, not every recipe.

## Press, selection, and hover

Give local acknowledgement at press initiation; commit according to component semantics, typically release/activation. Preserve cancel-by-moving-away where supported. Use a subtle scale, color, or depth change rather than transforming every interactive element. Keep keyboard selection responsive. Keep focus visibly identifiable and preserve touch affordances when hover enhancement is absent.

## Popover, tooltip, and anchored menu

Connect the surface to its trigger through placement and optional transform origin. Use a short opacity/near-final-size reveal if needed; a pure fade or immediate appearance can be appropriate. Respect collision-adjusted placement. Preserve valid focus/keyboard behavior and allow rapid open/close to retarget. Treat the initial tooltip delay independently; test movement among neighboring triggers.

## Modal, drawer, and sheet

Establish the layer with the surface and backdrop; keep the spatial relationship on dismissal. Keep a centered modal's origin centered when that matches its model. Preserve readable content and correct focus behavior. Distinguish blocking modal tasks from nonblocking panels. Use [gestures](gestures.md) for a draggable surface; glass styling is optional, not a motion requirement.

## Disclosure and conditional fields

Show what expanded and where it belongs. Keep a stable anchor; use a short expansion/fade or immediate reveal according to context. Measure actual layout cost if animating height. Preserve readable geometry instead of scaling text to fake expansion. Keep fields and their labels semantically available in the appropriate state.

## List insertion, removal, and reorder

Preserve item identity through stable keys and coherent destinations. Use a local entrance or position transition where users otherwise miss a change. Keep the rest of the list stable enough to inspect. Handle rapid updates and cancelled/failed mutations. Reconcile optimistic UI with confirmed state. Reserve stagger for cases where sequencing helps rather than delays reading.

## Data, filters, and dashboards

Update filters and active selection promptly. Preserve the table/chart shell, scroll context, and reading targets. Favor static results or restrained local transitions for dense/frequent work. Distinguish a decorative graph from data users must inspect; smoothing the cursor/data can obscure precision. Preserve truthful units, axes, values, and empty/error states.

## Loading → success/error

Keep a stable control/container where it preserves identity. Show real progress if measurable; use an indeterminate indicator/status otherwise. Avoid invented percentages or success before backend confirmation. Keep errors readable with a correction path. Handle cancellation, retry, rapid results, and slow/offline cases. Define the short-operation behavior to avoid an unnecessary spinner flash.

## Toast and notification

Use consistent edges/origins when they explain entry and dismissal. Support rapid stacking and removal from current state. Preserve readable messages and relevant actions, with accessible status behavior. Match timeout/control to the content's importance and task; animation settling does not determine how long a message remains available.

## Navigation, tabs, and shared elements

Keep repeated navigation prompt and usable. Distinguish a moving tab indicator from a sliding content pane; peers need not imply depth. Preserve a shared element only when both states represent the same object. Keep hierarchy/direction and return behavior coherent, including RTL. Static navigation and opacity-only changes are valid choices.

## Feature explanation and reward

Use setup → transformation → readable result. Preserve the product's actual capabilities. Keep utility controls and core text immediately available. Reward meaningful milestones selectively; retain a stable confirmation when motion is reduced. Add supporting movement only when it clarifies the main event.

## Ambient and scroll behavior

Keep low-priority atmosphere subordinate to reading and actions. Define loop length, pause/stop where applicable, offscreen suspension, and static composition. Distinguish one-time viewport triggers from scroll-linked scenes. Preserve native scroll, anchors, Back, fast/reverse scrolling, and content visibility if setup fails. Tune motion intensity by scene; personality archetypes and one-third ratios are composition aids, not requirements.
