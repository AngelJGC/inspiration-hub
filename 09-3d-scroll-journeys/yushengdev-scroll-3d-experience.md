# yushengdev/scroll-3d-experience

> **Tight "dive underwater" demo.** The narrative-scroll formula without the bloat.

- **URL:** https://github.com/yushengdev/scroll-3d-experience
- **Live:** https://scroll-3d-experience.vercel.app
- **Stars:** ⭐ 100+
- **Stack:** React Three Fiber · drei · GSAP · Lenis

## Techniques

- **Chapter-based scroll stages** — drei `<ScrollControls pages={N}>` fixes the scroll length.
- **Per-chapter HTML overlay** synchronized via `useScroll().offset` — text fades in/out at
  specific scroll ranges.
- **Shader-based ocean floor** with vertex displacement.
- **Post-processing chromatic aberration** ramping with depth.

## Why inspiring

The **"scroll into a world"** formula without the usual bloat: stages + HTML overlays + a few
post-FX. Under 1000 lines. Perfect template for documentary-style microsites, product stories,
"day in the life" agency scrollers.

## Cross-refs

- Production-scale equivalent: `basementstudio/scrollytelling` (06-editorial-scroll/).
