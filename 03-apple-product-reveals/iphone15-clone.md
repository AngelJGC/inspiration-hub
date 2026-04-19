# BackBenchDreamer/iphone15-site-clone

> **Lean Apple-clone variant.** Diff against adrianhajdin/iphone to learn structure.

- **URL:** https://github.com/BackBenchDreamer/iphone15-site-clone
- **Stack:** React · Vite · Three.js · GSAP · Tailwind · Sentry

## Techniques worth stealing

- **GLB rotation on scroll** — `useFrame` mutates `model.rotation.y` as `scrollY` changes.
- **Scroll-scrubbed camera** — `camera.position` interpolated via GSAP `ScrollTrigger.scrub`.
- **Color/variant picker** — clicking a swatch tweens material color with `gsap.to(mesh.material.color)`.
- **Simpler structure than adrianhajdin/iphone** — fewer components, easier to adapt.

## Why inspiring

Smaller codebase than the adrianhajdin original. If you're porting Apple-style reveals into an
existing app and don't want to scaffold a full site, this is the minimal kit.

## Cross-refs

- Parent pattern: `adrianhajdin-iphone` (full site).
- Compose with: `bmw-config` for a configurator layer on top.
