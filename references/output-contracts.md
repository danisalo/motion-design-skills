# Output contracts

Use the relevant contract; scale detail to the requested scope. Reuse existing output conventions and destinations. Keep findings and specifications self-contained; references may explain a rule but must not hide values/decisions needed for execution.

Lead with a compact decision table. Expand a full brief for complex gestures, asynchronous states, or disputed behavior; use concise rows for simple or intentionally static choices. State shared context, tokens, and equivalents once, then document local exceptions. Use one combined acceptance/verification matrix rather than repeating it under every behavior. In a design-only plan, label proposed checks as pending; reserve a detailed verification log for work actually exercised.

## Context record

Record target, requested outcome, audience/task, frequency, input/device, intended character, existing conventions, authorized changes, evidence available, and assumptions. Include only fields that affect decisions.

## Opportunity

Include location/trigger; communication gap; primary purpose; exposure; static alternative; add/keep/reduce/remove decision; proposed normal and reduced-motion behavior; priority; evidence status. Return a shortlist and rejected candidates with reasons.

## Finding

| Field | Required content |
|---|---|
| Severity | Blocking, functional, or polish |
| Location | Screen/component; file:line or recording moment when available |
| Evidence | Observed result or concrete static mechanism |
| Consequence | Task, control, accessibility, or readability effect |
| Correction | Specific changed behavior and relevant values/tokens |
| Acceptance | Observable check and needed input/device/motion modes |

Use blocking for task barriers, incorrect state, applicable accessibility failures, or severe demonstrated interruption. Use functional for worthwhile communication/continuity/performance corrections. Use polish for optional style refinement. Label a static performance risk as a risk; do not invent runtime severity.

## Motion brief

Write one brief per behavior, with a shared token definition for common values:

- Context, problem/evidence, primary purpose, and static alternative.
- Trigger; initial, intermediate, final, waiting/error, cancelled/reversed states as relevant.
- Properties, origin, path, displacement, stable anchors, and layering.
- Onset/delay, arrival, settling, input availability, and chosen curve/spring parameters.
- Sequence/overlap budget and reading holds when relevant.
- Rapid retriggering, reversal, cancellation, and system-state reconciliation.
- Reduced motion, static/setup-failure state, input equivalence, status/focus behavior.
- Observable acceptance checks and unresolved hypotheses.

Use exact proposed values when an implementer needs them; label them provisional until exercised. A human-only design brief can use a state/storyboard artifact instead of a source-file mapping.

## Beat sheet

Return message and focal subject, then a table: beat, communication purpose, focal movement, stable elements, duration/overlap, readable endpoint/hold. Add total budget, loop/replay/control rules, static explanation, and comprehension criteria.

## Verification

Report a table of check, result (passed/failed/unverified), and evidence/environment. Separate static review, runtime interaction, preference/input checks, and device/performance tests. Summarize changed decisions, known exceptions, and remaining evidence. Reserve “verified” for exercised criteria; lack of tool/device access is an unverified check rather than a pass.
