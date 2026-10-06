# Implement authorized motion

## 1. Resolve the behavior before changing code

Use an existing complete motion brief or run Design for unresolved decisions. Read [platforms](../references/platforms.md) and [performance](../references/performance.md), plus [timing](../references/timing.md), [patterns](../references/patterns.md), or [gestures](../references/gestures.md) for the behavior being implemented.

Inspect project dependencies, component semantics, and existing tokens. Choose the simplest installed mechanism that preserves the specified behavior. Add a dependency only when existing tools cannot satisfy the actual requirements and the task authorizes that change.

**Complete when:** target states, control behavior, accessible equivalents, mechanism, and acceptance criteria are fixed sufficiently to implement.

## 2. Make the smallest coherent change

Implement in the existing component/system. Keep semantic state authoritative; make visual transition lifecycle cleanup follow state. Implement normal, reduced-motion, and setup-failure paths together. Preserve focus, pointer targets, keyboard behavior, and status announcements where relevant.

For reversible behavior, retarget from the current presentation state. Release resources when components disappear or loops leave scope. Preserve static visibility and product use while animation code initializes or fails.

**Complete when:** each specified state and transition exists, interruption has a defined result, and motion does not alter the action's meaning or confirmed backend status.

## 3. Verify the behavior

Run project-required checks. Exercise normal and reduced motion, rapid retrigger/reversal, cancellation, error/waiting, and relevant input modes. Inspect geometry in screenshots and sequence/control in live interaction or recordings. Test under competing work and on weaker supported devices when available.

Use the verification contract in [outputs](../references/output-contracts.md), then run Review on the change. If runtime/device access is unavailable, finish available checks and mark those checks unverified; keep the change provisional rather than claiming verified delivery.

**Complete when:** available acceptance checks pass, failures are resolved, and remaining limitations are explicit.
