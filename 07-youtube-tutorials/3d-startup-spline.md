# MiladiCode/3D-startup-app

> **Cleanest minimal reference for dropping a Spline scene into a custom layout.**

- **URL:** https://github.com/MiladiCode/3D-startup-app
- **Live demo:** https://3-d-website-alpha.vercel.app
- **Video:** https://www.youtube.com/watch?v=oskiEydAaok — "Build a Stunning 3D Website with HTML, CSS & Spline"
- **Channel:** MiladiCode
- **Stack:** HTML · CSS · Spline (runtime viewer). **No React/Next.**

## Techniques worth stealing

- **Embedded Spline robot** — `<spline-viewer url="…">` custom element.
- **CSS-only layout** — zero JS framework overhead.
- **Animated 3D hero** — Spline's built-in runtime handles animation.

## Why inspiring

Starter to prove a hero concept before porting into a React/Next app. If the user wants a
Spline-based hero, first read this to understand the embed pattern, then port the scene URL
into a Next.js `<dynamic>` wrapper.

## Caveats

- Not a production template (plain HTML).
- Spline runtime is ~1 MB — test LCP before shipping.

## Cross-refs

- React version: wrap Spline in `@splinetool/react-spline` inside any of the Next.js portfolios
  in this hub.
