# Review a motion change

## 1. Bound the review

Read the diff/brief and affected shared patterns. Load [timing](../references/timing.md), [patterns](../references/patterns.md), and [performance](../references/performance.md); load [gestures](../references/gestures.md) for input-driven behavior and [platforms](../references/platforms.md) for platform-specific claims.

**Complete when:** every changed behavior, its stated purpose, and its consumers are identified, with static/runtime evidence distinguished.

## 2. Apply the quality gate

For every changed behavior, assess eligibility, prompt feedback, readable endpoint, input availability, origin/destination, interruption, normal/reduced-motion equivalence, applicable accessibility checks, rendering risk, and token/pattern consistency. Verify full sequence timing rather than just per-element duration.

Use the scoped requirement/default distinction in [principles](../references/principles.md). A default-range exception requires a reason and evaluation; classify an unsupported style preference as polish, not a blocker. Recheck cited evidence and respect intentional behavior unless its concrete consequence warrants a finding.

**Complete when:** each dimension has a finding, a supported pass, or an explicit unverified status; every finding has a reproducible mechanism and location.

## 3. Report a bounded verdict

Use finding and verification contracts in [outputs](../references/output-contracts.md). Report blocking issues first, then functional improvements and optional polish. State coverage and remaining checks. Use “verified” only for exercised acceptance criteria; otherwise say “static review complete; runtime verification pending.”

**Complete when:** the owner can distinguish necessary corrections, optional changes, and unavailable evidence. Apply corrections only when the task authorizes implementation.
