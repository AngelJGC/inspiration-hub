# pmndrs/react-postprocessing

> **Post-processing is what separates "a scene" from "a trailer".**

- **URL:** https://github.com/pmndrs/react-postprocessing
- **Live:** https://react-postprocessing.docs.pmnd.rs
- **Stars:** ⭐ 1k+
- **Stack:** React Three Fiber · postprocessing (Vanruesch)

## Effects

- **Selective bloom** via `<Selection>` / `<Select>` — only flag specific meshes to bloom.
- **Depth-of-field** with bokeh scale linked to scroll progress.
- **SSR (screen-space reflections)** and **GodRays** — the "premium" look.
- **LUT color grading** from `.cube` files exported from DaVinci Resolve / Premiere.

## Why inspiring

Wraps a powerful vanilla post-processing library in JSX that **composes cleanly with other R3F
libs**. Nothing ruins a 3D scene faster than the wrong color grade — LUT support means you can
treat your browser scene like cinema footage.

## Cross-refs

- Works inside any R3F scene: `pmndrs/react-three-next`, `pmndrs/drei`.
