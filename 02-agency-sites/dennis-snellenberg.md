# AliBagheri2079/dennis-snellenberg-portfolio

> **Faithful rebuild of Dennis Snellenberg's Awwwards-winning solo portfolio.** Magnetic cursor
> and page transitions are the headline features.

- **URL:** https://github.com/AliBagheri2079/dennis-snellenberg-portfolio
- **Stack:** Next.js · Framer Motion · GSAP · Lenis · Styled Components · Tailwind · Cloudinary

## Techniques worth stealing

- **Magnetic cursor** — a custom cursor that's attracted to buttons and interactive elements.
  Uses `framer-motion` `useMotionValue` + `animate()` with spring.
- **Staggered project reveal** — project cards slide up with `delay = index * 0.08`.
- **Page transitions** — full-page curtain wipe between routes, handled via Framer Motion's
  `AnimatePresence` + `mode="wait"`.
- **Cloudinary media pipeline** — auto-optimized WebP/AVIF via `f_auto,q_auto` URL params.
- **Preloader with SplitText** — letterform assembly on first load.

## Why inspiring

This is the **solo creative developer portfolio** template. The original site has been on
Awwwards SOTD lists multiple times. The rebuild uses every modern React trick (Next App Router,
Framer, GSAP, Lenis) without making them feel cluttered.

## Cross-refs

- Olivier Larose tutorials cover similar magnetic-cursor logic in plain React.
