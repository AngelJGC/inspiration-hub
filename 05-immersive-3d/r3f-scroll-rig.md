# 14islands/r3f-scroll-rig

> **The hidden weapon behind many Awwwards-winning hybrid DOM+WebGL sites.**

- **URL:** https://github.com/14islands/r3f-scroll-rig
- **Stars:** ⭐ 1.1k+
- **Stack:** React Three Fiber · Lenis

## Techniques worth stealing

- **Sync DOM elements to WebGL meshes** — `<ScrollScene>` + `<UseCanvas>` primitives let you
  wrap a regular `<img>` or `<h1>` and promote it to a 3D mesh with matching bounds.
- **Scroll-locked canvas** — single shared canvas driven by the same smooth scroll as the DOM.
- **Image-to-shader promotion** — turn any image into a GLSL-shaded plane without changing its
  layout position.
- **Performance-focused** — culls off-screen scenes automatically.

## Why inspiring

Essential when you want **NYT-style text storytelling *with* 3D accents** — text stays
accessible/SEO-friendly but specific elements upgrade to WebGL. This is how 14islands builds
their Awwwards projects (they're the studio behind this library).

## Cross-refs

- Compose with: `adrianhajdin-macbook` (anchor object) + `basement-scrollytelling` (text API).
- Alternative: `basement-scrollytelling` if you don't need WebGL.
