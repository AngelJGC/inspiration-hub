# adrianhajdin/threejs-portfolio

> **The "Awwwards-winning portfolio" crash course — R3F + GSAP pairing.**

- **URL:** https://github.com/adrianhajdin/threejs-portfolio
- **Video:** https://www.youtube.com/watch?v=E-fdPfRxkzQ — "Build and Deploy a Unique 3D Web Developer Portfolio with React, Three JS & GSAP"
- **Channel:** JavaScript Mastery (Adrian Hajdin)
- **Community mirror:** https://github.com/KpG782/3D_Portfolio
- **Stack:** React · Vite · Three.js · React Three Fiber · drei · GSAP (ScrollTrigger) · Tailwind

## Techniques worth stealing

- **Spaceship/planet hero** — animated 3D scene with camera movement.
- **Scroll-driven camera** — GSAP ScrollTrigger mutates `camera.position` per section.
- **Section-pinned scroll sequences** — like Apple events but for a portfolio.
- **Custom shaders** for starfield/nebula backgrounds.
- **Mobile fallback** — `useMediaQuery` swaps to a static image on small screens.

## Why inspiring

Combines R3F with GSAP ScrollTrigger — exactly the cross-library pairing most inspiration-hub
visitors want to learn. This is the sibling tutorial to `adrianhajdin-3d-portfolio` but uses
GSAP instead of Framer Motion, which is the preferred stack when scroll choreography is
mission-critical.

## Used in this showcase

- `06r-obsidiana` horno section — R3F canvas + GSAP scroll overlay is the pattern learned here.
