# adrianhajdin/iphone

> **The go-to reference for "Apple event" style product reveals.**

- **URL:** https://github.com/adrianhajdin/iphone
- **Live demo:** iphone-doc.vercel.app
- **Stars:** ⭐ 2k+ (approx)
- **Stack:** React · Vite · Three.js · React Three Fiber · drei · GSAP · Tailwind · Sentry

## Techniques worth stealing

- **Interactive 3D iPhone 15 Pro model** — real GLB loaded via drei `useGLTF`.
- **Color + size swap** — UI changes material on the same mesh instance (no reload).
- **Scroll-pinned video carousel** — multiple product videos sync to scroll progress.
- **GSAP timeline choreography** — hero → features → 3D → CTA all in one `gsap.timeline`.
- **Responsive 3D camera** — `gsap.matchMedia` adjusts camera for mobile/desktop.
- **Sentry error tracking** — shows how to instrument a motion-heavy site.

## Why inspiring

Apple's own iPhone page is the benchmark for product reveals; this repo rebuilds it with
modern React + R3F in ~3k lines. The GLB model and texture swap logic is ~100 lines and
portable to any product (car, watch, shoe, bottle).

## Used in this showcase

- `06r-obsidiana` reserva section — MeshTransmissionMaterial bottle uses the same drei
  `useGLTF` + material replacement pattern studied here.
