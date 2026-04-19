# 0xDigest/nft-landing-page

> **Tight, focused repo showing exact Lenis+GSAP wiring pattern most tutorials gloss over.**

- **URL:** https://github.com/0xDigest/nft-landing-page
- **Stars:** ⭐ 200+
- **Stack:** React · Vite · GSAP · Lenis · Tailwind CSS

## Techniques

- **Horizontal NFT carousel scrubbed by vertical scroll** — `ScrollTrigger.scrub: true`.
- **Lenis smooth-scroll hooked into ScrollTrigger** via `scrollerProxy` — the correct way.
- **SVG path drawing on scroll** — `strokeDashoffset` animation tied to progress.
- **Cursor-follow magnetic buttons** built on pointer deltas.

## Why inspiring

If you want to learn **exactly how Lenis and ScrollTrigger talk to each other**, this is the
cleanest 150-line reference on GitHub. The `scrollerProxy` pattern is what most "my Lenis is
jittery" issues boil down to.

## Used in this showcase

- `06r-obsidiana` pinned flavors slider uses the same scrub carousel pattern.
