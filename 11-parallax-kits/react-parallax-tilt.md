# mkosir/react-parallax-tilt

> **The canonical tilt library.** Clean reference if you'd rather write your own hook.

- **URL:** https://github.com/mkosir/react-parallax-tilt
- **Live:** https://react-parallax-tilt.vercel.app
- **Stars:** ⭐ 900+
- **Stack:** React · TypeScript

## Techniques

- **Pointer-driven 3D tilt** with configurable `tiltMaxAngle`.
- **Glare layer** using CSS conic/linear gradient positioned from angles.
- **Gyroscope support for mobile** (DeviceOrientation) — tilt follows phone orientation.
- **Composable with Framer Motion** by spreading tilt transforms into `motion.div`.

## Why inspiring

If you need a tilt-on-hover card, **don't roll your own** — use this or read the `Tilt.tsx`
source. The math (pointer position → `rotateX/rotateY` in degrees based on element bounds) is
the same pattern used in every premium NFT card, product showcase, and bento tile.

## Used in this showcase

- `06r-obsidiana` bento tiles use a from-scratch implementation inspired by this library's math.

## Cross-refs

- Applied in NFT context: `08-web3/piyush-nft-marketplace`.
