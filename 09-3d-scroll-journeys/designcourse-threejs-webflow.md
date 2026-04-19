# designcourse/threejs-webflow

> **The exact math for mapping scroll progress onto a spline-based camera path.**

- **URL:** https://github.com/designcourse/threejs-webflow
- **Stars:** ⭐ 200+
- **Stack:** Three.js (vanilla) · GSAP ScrollTrigger

## Techniques

- **Camera dolly along scroll-mapped `CatmullRomCurve3`** — the core trick behind every "scroll
  through a 3D world" site.
- **GLTF model broken into named meshes**, each with its own scroll timeline.
- **Scroll-tied lighting** — `directionalLight.intensity` = `useTransform(scroll)`.
- **Progressive environment map blend** — HDRIs crossfade with scroll progress.

## Why inspiring

Most tutorials hand-wave the "how do I move the camera smoothly through a 3D scene" question.
This repo shows the `CatmullRomCurve3.getPoint(t)` pattern that pros use — once you see it, you
see it in every major Awwwards 3D piece.

## Cross-refs

- Companion: `yomotsu/camera-controls` (09-3d-scroll-journeys/) — damping + fit-to-box helpers.
