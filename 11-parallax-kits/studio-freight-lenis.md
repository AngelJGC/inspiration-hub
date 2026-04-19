# darkroomengineering/lenis (formerly studio-freight/lenis)

> **Nearly every Awwwards site with "butter scroll" uses Lenis.**

- **URL:** https://github.com/darkroomengineering/lenis
- **Live:** https://lenis.darkroom.engineering
- **Stars:** ⭐ 9.8k+
- **Stack:** Vanilla JS + React/Vue wrappers

## Techniques

- **Smooth-scroll engine** feeding scroll progress into any parallax rig.
- **`normalizeWheel`** for cross-browser trackpad parity — this is the secret to "it feels the
  same on Mac and Windows".
- **`scrollerProxy` integration with GSAP ScrollTrigger** — the canonical way to pair the two.
- **Virtual scroll** for custom containers (not just `window`).

## Why inspiring

Pair Lenis with any parallax hook and you get **studio-grade feel for free**. If the user ever
says "why does this feel different from [agency site]?" — 80% of the time the answer is Lenis.

## Used in this showcase

- `showcase/reforge/components/lenis-singleton.ts` — used on every reworked page.
- `02r-milpa`, `06r-obsidiana` — both route through `getLenis()`.

## Cross-refs

- Its author's agency starter: `darkroomengineering/satus` (02-agency-sites/).
- Paired with: every entry in `11-parallax-kits/`.
