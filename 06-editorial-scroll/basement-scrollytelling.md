# basementstudio/scrollytelling

> **Production-grade abstraction from Basement Studio — the best React-idiomatic way to write
> NYT-style scroll pieces.**

- **URL:** https://github.com/basementstudio/scrollytelling
- **Stars:** ⭐ 2k+
- **Stack:** React · GSAP (ScrollTrigger wrapper) · TypeScript

## Techniques worth stealing

- **Declarative `<Root>` / `<Animation>` / `<Waypoint>` components** — wrap a section in
  `<Scrollytelling.Root>` and describe keyframes in JSX, not imperatively.
- **Typed timeline API** — TypeScript all the way; autocompletes tween properties.
- **Parallax primitive** — `<Scrollytelling.Parallax>` with `tween` prop.
- **Pinning primitive** — `<Scrollytelling.Pin>` handles ScrollTrigger internals.
- **Works inside any React tree** — no global state required.

## Why inspiring

This is what happens when a top motion-first studio productizes their internal toolkit. If
you're building a marketing page with complex scroll choreography and don't want to write
raw `gsap.timeline()` code, use this. Basement shipped the library in mid-2023 and it's now
a de-facto standard for React + scrolltelling.

## Cross-refs

- Lighter alternative: `react-kino` (more ready-made components, less flexibility).
- For pure editorial: pair with `02r-milpa` video-scrub pattern.
