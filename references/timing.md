# Timing and easing

## Starting ranges

Use existing project tokens first. When absent, use these provisional prototype values and test them in context:

| Moment | Range | Prototype value |
|---|---|---|
| Local press/selection feedback | 70–120ms | 100ms |
| Small popover/tooltip transition | 120–200ms | 160ms |
| Dropdown/small disclosure | 150–250ms | 180ms |
| Modal/drawer/larger disclosure | 200–300ms | 240ms |
| Explanatory scene | By beats and reading time | Specify per beat |

These are defaults, not limits or accessibility thresholds. Justify and verify longer UI movement by distance, purpose, and continued input availability. Treat hover activation delay separately from transition duration; after one toolbar tooltip is active, consider instant adjacent tooltips where the interaction supports it.

## Four clocks

Record onset/delay, meaningful arrival, total settling, and next-input availability. Visual settling can continue after an object becomes usable. Commit semantic state at the event appropriate to the action, not merely at a decorative animation's end.

For a uniform stagger of N elements: completion = (N − 1) × delay + duration. Record the entire sequence; 12 × 50ms offsets with 200ms transitions finish at 750ms. Start with a short group budget, commonly at most 400–500ms for utility content, or remove stagger where it delays reading.

## Easing vocabulary

| Behavior | Starting curve / model | Decision |
|---|---|---|
| Quick arrival | cubic-bezier(0.16, 1, 0.3, 1) | Prompt onset, soft landing |
| Visible reposition | cubic-bezier(0.4, 0, 0.2, 1) | Accelerate and settle |
| Permanent departure | cubic-bezier(0.2, 0, 1, 1) | Test a short accelerating exit |
| Reversible physical behavior | Retargetable spring without overshoot initially | Preserve state and velocity |
| Uniform-rate progress/rotation | linear when its rate has meaning | Preserve a consistent rate |

Depart promptly; a slow-looking exit onset may need a different curve. A panel resting nearby may decelerate toward its offscreen rest position instead of accelerating away. Built-in easing or opacity-only behavior can be adequate for a simple change; use custom curves when their difference serves the brief.

## Springs

Describe response, damping/overshoot, initial velocity, and settling tolerance. Start without overshoot for utility surfaces. Add restrained elasticity when momentum or the product's intended character supports it. Treat library “duration” options as library-specific tuning parameters; settle time can vary after new input. Verify the current library API before mapping damping, bounce, and response across systems.

## Amplitude and rest

Start small for local changes: approximately 4–12px travel or scale near 0.97→1 where scale communicates pressure/arrival. These are optional defaults; keep text and targets stable. Use larger travel only to explain location or structure. Give explanatory outcomes a reading hold; define it from the actual content rather than a fixed universal interval.
