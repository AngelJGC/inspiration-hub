# jscottsmith/react-scroll-parallax

> **De-facto React parallax library.** Its `useController` is a masterclass in sharing one RAF
> loop across many animated nodes.

- **URL:** https://github.com/jscottsmith/react-scroll-parallax
- **Live:** https://react-scroll-parallax.damnthat.tv
- **Stars:** ⭐ 1.9k+
- **Stack:** React 18+ · TypeScript

## Techniques

- **Unified `<ParallaxProvider>`** — a single scroll listener feeds all children (no N-listeners).
- **`useParallax` hook** with `startScroll` / `endScroll` windows per element.
- **Banner component** with `translateY` + `opacity` easing curves baked in.
- **SSR-safe** through conditional measurement.

## Why inspiring

If Rellax taught you the concept, this one shows you **how to scale parallax to dozens of
elements without tanking performance**. The single-RAF pattern is the critical insight.

## Cross-refs

- Primitive/educational version: `dixonandmoe/rellax`.
- For smooth scroll under it: `studio-freight/lenis`.
