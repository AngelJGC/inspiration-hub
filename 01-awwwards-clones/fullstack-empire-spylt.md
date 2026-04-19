# Fullstack-Empire/GSAP-Awwwards-Website

> **Community rebuild of an Awwwards SOTD, pure GSAP choreography focus.**

- **URL:** https://github.com/Fullstack-Empire/GSAP-Awwwards-Website
- **Stack:** React · Tailwind · GSAP (ScrollSmoother, ScrollTrigger, SplitText)

## Techniques worth stealing

- **ScrollSmoother + Lenis combo** — butter-smooth wheel inertia.
- **Horizontal scroll panels** — pinned section with `x: -scrollLen` translation.
- **Marquee strips** — infinite horizontal text ribbons used as section dividers.
- **Kinetic typography** — headers that scale / slide / split on scroll.
- **Image reveal on enter** — `clipPath: inset(…)` animated from full-inset to zero.

## Why inspiring

Where adrianhajdin's repos teach you structure, this one teaches you **choreography**. Every
scroll interaction is hand-tuned. Read the `gsap.context()` blocks — the timeline composition
is a masterclass.

## Used in this showcase

- `06r-obsidiana` — every GSAP pattern in ObsidianaClient (scrub timelines, pinned flavors,
  kinetic manifiesto) was studied from this repo before adapting.
