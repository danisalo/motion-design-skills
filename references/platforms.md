# Platform selection

## Web and PWA

Use the smallest existing mechanism that satisfies the brief:

| Behavior | Mechanism to consider |
|---|---|
| Small state-driven visual change | CSS transition or an installed component primitive |
| Reversible discrete animation | CSS transition, WAAPI retargeting, or installed animation library |
| Gesture with velocity / shared identity | Existing gesture/spring/layout primitive |
| Multi-beat explanatory scene | Existing timeline library or a contained timeline |
| Authored illustration | Existing Lottie/Rive/SVG asset/player when available and suitable |

Implement touch, keyboard, and pointer behavior where the product supports them. Preserve static visibility and native navigation/scroll semantics. Verify support before using newer CSS features; provide an immediate usable fallback. Avoid introducing a motion library merely to replace a simple existing transition.

## React Native / Expo

Inspect installed versions and native primitives. Prefer platform navigation, tabs, sheets, menus, and refresh behavior when they satisfy the task. For custom gestures, keep continuous tracking and settling on the appropriate UI runtime. Reanimated/Gesture Handler are options when already available or justified; inspect their current APIs instead of copying a version-specific recipe.

Use release-build behavior on supported devices to validate performance when access permits. Handle platform reduced-motion settings and supported input alternatives. Add haptics only for a meaningful event, synchronized with its actual state; preserve visual information independently.

## Translate intent, not an aesthetic package

An Apple-style spring does not require translucent chrome. A native sheet recipe is not automatically a browser dialog recipe. An authored video is not a gesture-driven component. Preserve the purpose/state/control contract, then select the implementation supported by the actual environment.
