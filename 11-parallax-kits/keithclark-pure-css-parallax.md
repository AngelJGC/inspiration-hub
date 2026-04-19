# keithclark/pure-css-parallax-demos

> **Keith Clark's seminal article + demos.** The lightest way to ship parallax, and the
> conceptual foundation under most JS libs.

- **URL:** https://github.com/keithclark/pure-css-parallax-demos
- **Live:** https://keithclark.co.uk/articles/pure-css-parallax-websites/demo3/
- **Stack:** **Pure CSS — no JavaScript.**

## Techniques

- **`perspective` + `transform: translateZ(-Npx) scale(N)`** multi-layer rig.
- **Per-layer `translateZ` depths** mapped to perceived speed (deeper = slower).
- **Zero-JS sticky headers** that respect parallax viewport.

## Why inspiring

From 2014, and **still the reference**. If the user cares about performance (mobile, low-end
devices), CSS parallax is the answer. Zero JS means zero RAF overhead. The trade-off: static
depth layers — no dynamic scroll-linked transforms.

## Article worth reading

https://keithclark.co.uk/articles/pure-css-parallax-websites/ — the explanation of why the
math works at all is a great mental model.

## Cross-refs

- When CSS isn't enough → `react-scroll-parallax` + `lenis`.
