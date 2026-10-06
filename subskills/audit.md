# Audit existing motion

## 1. Inventory the current system

Map the requested screens, existing duration/easing tokens, component patterns, animation mechanisms, input modes, and frequently repeated actions. Reuse documented intent as context. Read [patterns](../references/patterns.md), [timing](../references/timing.md), and [performance](../references/performance.md); read [gestures](../references/gestures.md) where movement follows input.

**Complete when:** coverage, existing conventions, and available runtime evidence are recorded; each observed animation has a location and trigger.

## 2. Evaluate behavior and gaps

Evaluate purpose/frequency, onset/arrival/availability, spatial identity, interruption, readability, accessibility, rendering cost, and consistency. Inspect runtime behavior where possible. For static findings, identify the code and causal mechanism without inventing measured delay, frame loss, or user reactions.

Evaluate absent motion only when a specific communication gap exists. Consider a static correction and removal of existing motion alongside adding effects.

**Complete when:** every in-scope behavior has been assessed or explicitly marked uncovered; each finding has confirmed evidence, consequence, and proposed correction.

## 3. Prioritize an actionable plan

Use the finding contract in [outputs](../references/output-contracts.md). Order by severity, then breadth and implementation effort. Deduplicate shared-component defects. Preserve intentional tradeoffs unless evidence shows their consequence. Separate product barriers from optional style preferences.

For each accepted change, name its behavior, token reuse or proposed value, accessible equivalent, and verification criteria. Hand off to Design for unresolved decisions or Implement when changes are authorized.

**Complete when:** findings, keep/remove decisions, coverage, and unverified checks are reviewable; each planned change is self-contained.
