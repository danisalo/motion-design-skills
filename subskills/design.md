# Design motion behavior

## 1. Set the communication goal

Use the eligibility gate in [principles](../references/principles.md). Identify the user's task, primary purpose, frequency, input modes, and intended character. Separate utility controls from expressive demonstration areas.

**Complete when:** the motion decision has a stated problem and a static alternative; stillness is recorded where it wins.

## 2. Specify the state behavior

Read [patterns](../references/patterns.md) and [timing](../references/timing.md); read [gestures](../references/gestures.md) for direct manipulation. Define states, trigger, origin/path, changed properties, stable anchors, timing/settling, and input availability. Include cancellation, retriggering, reversal, asynchronous failure, and reduced-motion behavior.

For a system, reuse existing tokens or propose a compact vocabulary: fast/standard/large durations, arrival/reposition/departure curves, and a restrained spring. Define different intensity by task; preserve semantic consistency rather than one identical effect everywhere.

**Complete when:** every accepted behavior has a complete motion brief, and shared decisions have one authoritative token/pattern definition.

## 3. Make the design reviewable

Use the specification contract in [outputs](../references/output-contracts.md). Provide a prototype if the request and environment support one; otherwise give a human-executable storyboard or state specification. Compare instant/static, restrained, and expressive variants only where that comparison resolves an actual choice.

**Complete when:** the brief includes observable acceptance criteria, named provisional values, and the evidence needed to validate remaining hypotheses. Claim user benefits only to the extent supported by evaluation.
