# adrianhajdin/award-winning-website

> **Zentry clone — Awwwards Site Of The Month.** The canonical reference for bold kinetic landing pages.

- **URL:** https://github.com/adrianhajdin/award-winning-website
- **Live demo:** https://award-winning-website-phi.vercel.app
- **Stars:** ⭐ 2.3k+ (approx)
- **Stack:** React 18 · Vite · GSAP 3 (ScrollTrigger) · Tailwind CSS · clsx
- **Video build-along:** JavaScript Mastery — "Build and Deploy an Award-Winning Website"

## Techniques worth stealing

- **Circular clip-path section reveal** — the signature Zentry move. Video or image is masked by a
  circle whose radius scales from 120% → 0% on scroll, revealing the next section like a keyhole.
- **3D tilt hover on bento cards** — `rotateX/Y` + `transformPerspective: 500` driven by
  `mousemove` relative to the card bounds.
- **Looping autoplay video as hero fill** — muted `<video>` with `object-fit: cover` + GSAP scale
  on enter.
- **Scroll-pinned story beats** — each chapter `pin: true` + `scrub: 1` for camera-like pacing.
- **Kinetic typography with SplitText** — per-character stagger + scroll-scrub on the hero header.

## Why inspiring

The original Zentry site won SOTM; this rebuild is the most viewed open-source replication.
Nearly every "bento + clip-path + pinned" landing page on 2025–2026 Awwwards shortlists traces
back to techniques demoed here. If you have one React+GSAP repo to read, make it this one.

## Used in this showcase

- `showcase/reforge/components/sites/06r/ObsidianaClient.tsx` — hero clip-path circle reveal,
  bento tilt cards, pinned flavors slider.
