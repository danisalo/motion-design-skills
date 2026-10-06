# Runtime performance and verification

## Mechanism and rendering

Prefer transform/opacity for cheap visual movement. Treat compositor-friendly rendering and off-main-thread animation as distinct properties. Inspect the actual library implementation and browser behavior; transform shorthands, CSS variables, clipping, filters, and acceleration support can differ by version.

For height/width or paint-heavy effects, measure the affected subtree, layer area, concurrent work, and visual alternatives. A contained layout transition can be acceptable; transform/opacity are not free or unlimited. Choose readable geometry over an unmeasured optimization that distorts content.

Use layer promotion/will-change only where measurement warrants it and release transient hints afterward. Stop unnecessary loops offscreen/backgrounded and clean up listeners, timelines, frames, and gesture resources. Keep animation state local to the mechanism rather than forcing component rerenders per frame when it creates avoidable work.

## Platform constraints

On native, prefer installed native/UI-runtime primitives for gesture and frame-critical work. On web, choose CSS/WAAPI/library behavior appropriate to interruption and input. Use the project's framework and installed tools; verify current APIs only for the platform branch being changed.

## Evidence

- **Static:** code inspection can identify a layout pass, unbounded properties, missing cleanup, or an acceleration risk. Label it as such.
- **Runtime:** recordings and interaction establish visible sequence, response, interruption, and artifacts in the exercised environment.
- **Device:** measurements under competing work on supported devices establish performance there; a fast desktop does not validate a weaker mobile device.

For each changed runtime behavior, inspect normal and busy cases. At 60Hz the entire frame has about 16.7ms; at 120Hz about 8.3ms. These are total frame budgets, not allowances entirely assigned to animation code. Record observed long frames or bottlenecks rather than asserting a guaranteed FPS from a property choice.

## Verification sequence

Check endpoints/geometry → play normally → inspect slow motion for discontinuities → rapidly interact/reverse → exercise reduced motion and failure → test competing work and relevant devices. Use existing project checks for state/semantic correctness. Report passed, failed, and unverified checks independently.
