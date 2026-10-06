# Continuous gesture behavior

## Tracking

Follow the pointer/finger directly while held, respecting the initial grab offset. Use the platform's pointer capture or gesture ownership mechanism. Resolve gesture intent with a small context-appropriate threshold while preserving native scrolling and cancellation. Separate gesture acknowledgement from the eventual commit.

## Release and settling

Track recent position/time samples to estimate release velocity in the units expected by the implementation. Combine position, direction, release velocity, valid snap targets, and cancellation rules. A fast short flick and a slow committed drag may both be valid; a single hard-coded velocity threshold is not a universal dismissal rule.

Project the likely endpoint when it helps the interaction, then settle to a valid target from the current presentation position with velocity handoff. Prefer an installed/native primitive with reliable behavior over reproducing platform physics formulas from memory.

## Interruption

Allow a surface to be grabbed, redirected, or reversed while settling where the task permits it. Retarget from the current visible value rather than the last logical destination; preserve velocity when continuity requires it. Distinguish continuous gesture tracking from decorative cursor-following, where deliberate smoothing may be acceptable.

Use increasing resistance at boundaries when it communicates a limit. Keep the valid range discoverable and actions reachable. Define what happens if the pointer cancels, the viewport changes, or the component disappears mid-gesture.

## Verification

Exercise slow drag, fast flick, short release, cancellation, boundary overshoot, interrupted settling, and direction reversal. Confirm the surface neither jumps nor finishes an obsolete trajectory before responding. Test click/tap alternatives and keyboard support separately. Record actual target-selection outcomes, not just frame rate.
