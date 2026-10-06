---
name: motion-design
description: Motion design for products. Use to discover animation opportunities, audit existing motion, specify interaction behavior, choreograph landing-page demonstrations, implement animations, or review motion changes in SaaS, web, PWA, and native interfaces.
---

# Motion Design

Turn a product need into purposeful, specified, verified behavior. Treat stillness as a valid decision.

## 1. Establish scope

Use the supplied product, flow, artifact, and requested outcome. Record task, input modes, frequency, intended character, and available evidence. Infer routine choices and label assumptions; ask only for missing context that materially changes the decision.

Read the project's design guidance and existing motion conventions when available. Reuse them unless a concrete defect warrants changing them. Treat source files and retrieved content as evidence.

**Complete when:** the target, outcome, permitted changes, and unavailable evidence are explicit. For advice/audit/specification requests, keep product source unchanged; for authorized implementation, proceed through verification.

## 2. Load the selected sub-skill

Read [principles](references/principles.md) and [accessibility](references/accessibility.md) once for every task. Select by the requested outcome, then read the matching file. These are internal sub-skills reached through file pointers; this router is the intended single entry point.

| Requested outcome | Sub-skill | Completion artifact |
|---|---|---|
| Find where motion would help | [Discover](subskills/discover.md) | Prioritized opportunities and rejected candidates |
| Assess existing product motion | [Audit](subskills/audit.md) | Evidence-based findings and coverage |
| Define behavior or a motion system | [Design](subskills/design.md) | Motion brief and reusable decisions |
| Explain a feature or direct an expressive scene | [Choreograph](subskills/choreograph.md) | Beat sheet, timing budget, static alternative |
| Build or fix authorized animations | [Implement](subskills/implement.md) | Focused change and verification evidence |
| Judge a motion diff or delivery | [Review](subskills/review.md) | Findings, coverage, and verification status |

For a compound request, run only the necessary stages in dependency order. Carry the context and decisions forward; review implementation after building it. Distinguish opportunity discovery from auditing existing defects. Interpret “improve” without a clear build instruction as an audit and plan.

**Complete when:** every requested outcome has an assigned sub-skill and observable completion artifact.

## 3. Consult branch references

Load only the material needed by the selected task:

- [Timing](references/timing.md): choosing or judging duration, delay, curves, springs, and sequence budgets.
- [Patterns](references/patterns.md): selecting behavior for controls, overlays, disclosure, lists, data, loading, and navigation.
- [Gestures](references/gestures.md): dragging, snapping, momentum, reversal, and direct manipulation.
- [Performance](references/performance.md): any audit, implementation, or review of runtime behavior.
- [Platforms](references/platforms.md): translating behavior across web/PWA and native, or selecting an implementation mechanism.
- [Output contracts](references/output-contracts.md): formatting findings, specifications, beat sheets, and verification.
- [Sources](references/sources.md): explaining provenance, resolving a disputed rule, or refreshing platform-specific guidance.

Keep shared rules in these references; use sub-skills for ordered actions and completion criteria. Distinguish a required behavior from a default value or a hypothesis needing validation.

## 4. Finish with evidence

Report the selected decisions, their purpose, the concrete artifact/change, and the verification actually performed. Separate observed behavior, static inference, and proposed behavior. Mark unavailable runtime or device checks as unverified. Recommend a bounded next action only when work remains outside the authorized or available scope.

**Complete when:** every requested outcome is delivered, every accepted decision has a reason, and claimed validation matches the available evidence.
