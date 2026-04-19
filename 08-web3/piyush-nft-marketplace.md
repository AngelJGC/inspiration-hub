# PiyushKumar-dev/NFT-Marketplace-Landing-Page

> **Compact reference for productionizing the "tilted NFT card grid" look.**

- **URL:** https://github.com/PiyushKumar-dev/NFT-Marketplace-Landing-Page
- **Live:** https://nft-marketplace-piyush.vercel.app
- **Stars:** ⭐ 100+
- **Stack:** Next.js · Tailwind · Framer Motion

## Techniques

- **Tilt-on-hover NFT cards** via `react-parallax-tilt` with glare.
- **Section entrance orchestrated by shared `containerVariants` object**.
- **Gradient border animation** — conic-gradient + `@property --angle`.

## Why inspiring

The OpenSea-style card grid pattern, distilled. The `@property --angle` trick for animated
conic gradients is a CSS gem — modern browsers only, but gorgeous.

## Cross-refs

- Tilt library itself: `mkosir/react-parallax-tilt` (11-parallax-kits/).
