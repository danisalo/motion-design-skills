# Motion Design Skills

Purposeful motion for SaaS, web, PWA, and native interfaces: find opportunities, assess existing animations, specify behavior, choreograph demonstrations, implement changes, and review delivery. Stillness is a valid outcome.

## Macro skill: `motion-design`

[SKILL.md](SKILL.md) is the single entry point. It establishes scope, loads the relevant workflow and references, and delivers decisions backed by evidence. Compound requests run only the necessary stages in dependency order; implementation ends with review.

Every workflow considers accessibility, reduced motion, truthful state, and user control. Existing project conventions take priority; runtime and device checks that were unavailable are reported as unverified.

## How to use it

Make the **whole folder** available to your agent as a skill, preserving `SKILL.md`, `subskills/`, and `references/`. The router relies on those relative links.

Explicitly request `motion-design` and describe the outcome, target screen/component/flow, and available evidence (source, screenshots, recordings, or a live interface). State whether you want advice, a specification, or implementation.

> Use motion-design to audit the checkout flow. Prioritize accessibility and repeated interactions; return findings and a plan.

The skill description also enables automatic selection for relevant motion requests when the agent supports it. The six sub-skills are internal Markdown workflows selected by the router, rather than separately registered skills or slash commands. Name a workflow in your request to select it explicitly.

## Individual workflows


| Workflow                                | Deliverable                                                                                                                                         | Example invocation                                                                                  |
| --------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------- |
| [Discover](subskills/discover.md)       | Find communication gaps where motion helps. Return up to five prioritized opportunities, static alternatives, and rejected candidates.              | “Use motion-design to discover animation opportunities in onboarding.”                              |
| [Audit](subskills/audit.md)             | Assess existing motion for usability, accessibility, consistency, and performance. Return evidence-based findings, coverage, and a correction plan. | “Use motion-design to audit the dashboard’s existing animations.”                                   |
| [Design](subskills/design.md)           | Specify states, triggers, timing, interruption, and accessible equivalents. Return motion briefs or a compact reusable motion system.               | “Use motion-design to design drawer behavior, including reversal and reduced motion.”               |
| [Choreograph](subskills/choreograph.md) | Explain a feature through setup → transformation → result. Return a beat sheet, total timing budget, replay/control rules, and static alternative.  | “Use motion-design to choreograph a landing-page demo of our filtering feature.”                    |
| [Implement](subskills/implement.md)     | Build or fix specified motion with existing project tools. Resolve missing design decisions, make a focused change, verify, then review it.         | “Use motion-design to implement the drawer animation and verify reduced motion and rapid toggling.” |
| [Review](subskills/review.md)           | Judge a motion diff or delivery against its brief. Return blockers, functional improvements, optional polish, and verification status.              | “Use motion-design to review this animation diff against the motion brief.”                         |


**Scope:** Discover finds opportunities; Audit assesses the existing system; Review assesses a change or delivery. Advice, audits, and specifications leave product source unchanged. “Improve animations” without a clear build instruction produces an audit and plan; request implementation explicitly to change code.

For a combined task:

> Use motion-design to audit the settings drawer, design corrections, implement them, and review the result.



## Shared references

These support the workflows; they are not additional skills. [Principles](references/principles.md) and [accessibility](references/accessibility.md) load for every task. The rest load as needed.


| Reference                                          | Used for                                                                                               |
| -------------------------------------------------- | ------------------------------------------------------------------------------------------------------ |
| [Principles](references/principles.md)             | Decide whether motion earns its place; distinguish requirements, defaults, and hypotheses.             |
| [Accessibility](references/accessibility.md)       | Reduced-motion equivalents, input/focus semantics, user control, and applicable accessibility checks.  |
| [Timing](references/timing.md)                     | Durations, easing, springs, delays, and full sequence budgets; values are provisional starting points. |
| [Patterns](references/patterns.md)                 | Behavior recipes for controls, overlays, lists, data, loading, navigation, and expressive scenes.      |
| [Gestures](references/gestures.md)                 | Direct tracking, release velocity, snapping, cancellation, and interrupted settling.                   |
| [Performance](references/performance.md)           | Rendering cost, cleanup, runtime/device checks, and evidence limits.                                   |
| [Platforms](references/platforms.md)               | Choose existing web/PWA or native mechanisms that satisfy the behavior.                                |
| [Output contracts](references/output-contracts.md) | Formats for opportunities, findings, motion briefs, beat sheets, and verification.                     |
| [Sources](references/sources.md)                   | Provenance, contextual adaptations, and guidance for resolving disputed rules.                         |


