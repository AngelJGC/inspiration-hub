# adrianhajdin/gsap_macbook_landing

> **Baseline reference for any "Apple-on-scroll" hero.**

- **URL:** https://github.com/adrianhajdin/gsap_macbook_landing
- **Stack:** React · Vite · Three.js · GSAP · Tailwind

## Techniques worth stealing

- **MacBook lid opening on scroll** — scroll progress drives `rotation.x` of the lid mesh.
- **Scene transition from 3D → flat hero** — camera dolly + fade to 2D product shot.
- **Scroll-pinned section** with GSAP ScrollTrigger `pin: true`.
- **Image trail** — product gallery that scrolls horizontally inside the MacBook screen.

## Why inspiring

Demonstrates the "anchor object" technique — one hero 3D model that choreographs the entire
scroll experience. Used in many 2024-2026 Awwwards winners (think Cartier, Rimowa).

## Cross-refs

- Alternative: `adrianhajdin-iphone` (full product reveal).
- Scaling up: pair with `r3f-scroll-rig` to sync DOM text with the 3D model.
