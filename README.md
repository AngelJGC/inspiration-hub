# Inspiration Hub — React · GSAP · Three.js landing pages

> Curated library of high-quality open-source landing pages, portfolios, agency sites, Web3
> showcases, 3D journeys, parallax rigs and motion libraries.
> Built as a reference for future AI coding sessions (Claude, Cursor, etc.) when the user asks
> for a new landing page and wants it inspired by the best-in-class work on GitHub.

**Current count:** 48 repos across 12 categories.

📎 **Also see: [`ASSETS.md`](ASSETS.md)** — where these repos get their images, 3D models,
fonts, audio, and the modern AI tools (Nano Banana, Midjourney v7, Flux, Ideogram 3, Runway
Gen-4, Meshy, DepthAnything V2, etc.) for sourcing hero material.

---

## Purpose

When the user asks for a new landing page or marketing site, **start here**. Every entry has
been vetted for:

- High star count and active maintenance
- Modern stack (React / Next.js / Three.js / GSAP / Framer Motion / Lenis)
- A named, recognisable technique worth stealing
- A recreatable result — not just a pretty demo, but code you can learn from

This repo was born from the **Obsidiana mezcal redesign** (Apr 2026). Every subsequent entry
extends that vocabulary across new domains (Web3, pure 3D journeys, parallax, etc.).

---

## How to use (for AI agents)

1. Read this README to get the category map.
2. Pick 2–3 repos whose techniques match the brief (e.g. "scroll into 3D world" →
   `09-3d-scroll-journeys/`, "Web3 landing" → `08-web3/`).
3. Read each repo's `.md` ficha — stack, techniques, why inspiring, cross-refs.
4. Clone the URL only when you need full source.
5. Cross-reference with the **Techniques Matrix** below to avoid duplicating a pattern.

---

## Categories

| #  | Folder                      | Vibe                                     | Best for                                        |
| -- | --------------------------- | ---------------------------------------- | ----------------------------------------------- |
| 01 | `01-awwwards-clones/`       | SOTM / SOTD rebuilds                     | Bold kinetic hero, clip-path, scroll-pin        |
| 02 | `02-agency-sites/`          | Studio / agency landings                 | Magnetic cursor, grid hover, transitions        |
| 03 | `03-apple-product-reveals/` | Apple event / iPhone clones              | 3D GLB, scroll-scrubbed camera, variants        |
| 04 | `04-creative-portfolios/`   | Dev + designer portfolios                | Preloader, project strip, case studies          |
| 05 | `05-immersive-3d/`          | WebGL product + configurators            | R3F, drei, HDRI, shader materials               |
| 06 | `06-editorial-scroll/`      | NYT-style scrollytelling                 | Video scrub, waypoint-driven prose              |
| 07 | `07-youtube-tutorials/`     | Repos from YouTube build-along videos    | Beginner-friendly full builds                   |
| 08 | `08-web3/`                  | Crypto / NFT / DeFi landings             | Glassmorphism, token ticker, tilted cards       |
| 09 | `09-3d-scroll-journeys/`    | Scroll-through-a-3D-world experiences    | Camera dolly on spline, baked lighting          |
| 10 | `10-framer-showcase/`       | Framer Motion libraries + showcases      | Layout animations, shared elements, bento       |
| 11 | `11-parallax-kits/`         | Parallax engines + tilt libraries        | Multi-layer depth, smooth scroll, tilt cards    |
| 12 | `12-threejs-art/`           | Pure Three.js / R3F art pieces           | Shaders, GPGPU, physics, post-FX, depth maps    |

---

## Techniques Matrix

| Technique                          | Primary reference                                    |
| ---------------------------------- | ---------------------------------------------------- |
| Zentry-style clip-path reveal      | `01-awwwards-clones/adrianhajdin-award-winning`      |
| Spylt kinetic typography           | `01-awwwards-clones/fullstack-empire-spylt`          |
| Video-masked section reveal        | `01-awwwards-clones/adrianhajdin-gta-vi`             |
| SplitText character scrub          | `01-awwwards-clones/adrianhajdin-cocktails`          |
| Stacked panels with rounded corners| `01-awwwards-clones/olivierlarose-nextjs-awwwards`   |
| Awwwards recipes cookbook          | `01-awwwards-clones/olivierlarose-youtube-tutorials` |
| TikTok-viral microinteractions     | `01-awwwards-clones/tomisloading-tutorials`          |
| Awwwards homepage grid itself      | `01-awwwards-clones/codegrid-awwwards-clone`         |
| 3D product variant picker          | `03-apple-product-reveals/adrianhajdin-iphone`       |
| Scroll-pinned horizontal panels    | `01-awwwards-clones/fullstack-empire-spylt`          |
| Magnetic cursor + page transitions | `02-agency-sites/dennis-snellenberg`                 |
| Agency-grade Next.js starter       | `02-agency-sites/darkroom-satus`                     |
| DOM↔WebGL sync (hybrid 3D/text)    | `05-immersive-3d/r3f-scroll-rig`                     |
| Scrollytelling primitives (React)  | `06-editorial-scroll/basement-scrollytelling`        |
| Scrollytelling primitives (v2)     | `06-editorial-scroll/react-kino`                     |
| Car configurator                   | `05-immersive-3d/bmw-config`                         |
| Apple MacBook scroll landing       | `03-apple-product-reveals/adrianhajdin-macbook`      |
| **Web3 / NFT hero**                | `08-web3/nyxb-cryptoui`                              |
| **Lenis + GSAP exact wiring**      | `08-web3/0xdigest-nft-landing`                       |
| **Floating coin / crypto asset**   | `08-web3/aditya-crypto-landing`                      |
| **Tilted NFT card grid**           | `08-web3/piyush-nft-marketplace`                     |
| **Camera dolly on spline curve**   | `09-3d-scroll-journeys/designcourse-threejs-webflow` |
| **Baked Blender lighting**         | `09-3d-scroll-journeys/bruno-simon-my-room`          |
| **Next.js 14 + R3F (no flash)**    | `09-3d-scroll-journeys/pmndrs-react-three-next`      |
| **Pro camera damping / fitToBox**  | `09-3d-scroll-journeys/yomotsu-camera-controls`      |
| **Scroll-into-a-world narrative**  | `09-3d-scroll-journeys/yushengdev-scroll-3d-experience` |
| **`layout` / `layoutId` FLIP**     | `10-framer-showcase/framer-motion-examples`          |
| **Framer tutorial library**        | `10-framer-showcase/olivierlarose-framer-motion-tutorials` |
| **Restrained Framer in shadcn**    | `10-framer-showcase/shadcn-ui`                       |
| **Animated Beam / Orbiting / Spotlight** | `10-framer-showcase/magicui`                  |
| **AI/SaaS 2026 aesthetic**         | `10-framer-showcase/aceternity-ui`                   |
| **Parallax minimal engine**        | `11-parallax-kits/dixonandmoe-rellax`                |
| **React parallax at scale**        | `11-parallax-kits/react-scroll-parallax`             |
| **Butter-smooth scroll (Lenis)**   | `11-parallax-kits/studio-freight-lenis`              |
| **Tilt card / glare**              | `11-parallax-kits/react-parallax-tilt`               |
| **Pure CSS parallax**              | `11-parallax-kits/keithclark-pure-css-parallax`      |
| **R3F glass / caustics / float**   | `12-threejs-art/pmndrs-drei`                         |
| **Bloom / DOF / LUT grading**      | `12-threejs-art/pmndrs-react-postprocessing`         |
| **R3F examples index**             | `12-threejs-art/pmndrs-r3f-examples`                 |
| **Rapier physics playground**      | `12-threejs-art/pmndrs-react-three-rapier`           |
| **GPGPU particle fluid**           | `12-threejs-art/edankwan-the-spirit`                 |
| **Depth-map fake-3D photo**        | `12-threejs-art/akella-fake3d`                       |

---

## Index (one-line per repo)

### 01 — Awwwards clones (9)
- **[adrianhajdin/award-winning-website](01-awwwards-clones/adrianhajdin-award-winning.md)** — Zentry SOTM rebuild (⭐ 2.3k+)
- **[adrianhajdin/jsm_gta_vi_landing](01-awwwards-clones/adrianhajdin-gta-vi.md)** — GTA VI trailer landing (⭐ 500+)
- **[adrianhajdin/gsap_cocktails](01-awwwards-clones/adrianhajdin-cocktails.md)** — Beverage brand SplitText reveal (⭐ 300+)
- **[Fullstack-Empire/GSAP-Awwwards-Website](01-awwwards-clones/fullstack-empire-spylt.md)** — Community Spylt/Awwwards rebuild
- **[Zentry clone swarm](01-awwwards-clones/zentry-clone-swarm.md)** — 4 community variants
- **[olivierlarose/nextjs-awwwards-tutorial](01-awwwards-clones/olivierlarose-nextjs-awwwards.md)** — Stacked panel aesthetic (⭐ 400+)
- **[olivierlarose/youtube-tutorials](01-awwwards-clones/olivierlarose-youtube-tutorials.md)** — 30+ recipe cookbook (⭐ 1.1k+)
- **[tomis5y/tomis-tutorials](01-awwwards-clones/tomisloading-tutorials.md)** — TikTok-viral microinteractions
- **[CodeGrid/awwwards-clone](01-awwwards-clones/codegrid-awwwards-clone.md)** — Literal Awwwards rebuild (⭐ 300+)

### 02 — Agency / studio sites (5)
- **[Sankalp20Tiwari/spylt](02-agency-sites/sankalp-spylt.md)** — Tubik Spylt rebuild
- **[AliBagheri2079/dennis-snellenberg-portfolio](02-agency-sites/dennis-snellenberg.md)** — Awwwards solo-dev
- **[Shatlyk1011/agency-website](02-agency-sites/shatlyk-agency.md)** — Next.js + Framer agency
- **[awwwards-inspired topic](02-agency-sites/awwwards-inspired-topic.md)** — Ochi / k72 clones
- **[darkroomengineering/satus](02-agency-sites/darkroom-satus.md)** — Pro agency Next.js starter (⭐ 600+)

### 03 — Apple-product-style reveals (3)
- **[adrianhajdin/iphone](03-apple-product-reveals/adrianhajdin-iphone.md)** — iPhone 15 Pro R3F (⭐ 2k+)
- **[BackBenchDreamer/iphone15-site-clone](03-apple-product-reveals/iphone15-clone.md)** — Lean iPhone clone
- **[adrianhajdin/gsap_macbook_landing](03-apple-product-reveals/adrianhajdin-macbook.md)** — MacBook hero

### 04 — Creative portfolios (3)
- **[ayush013/folio](04-creative-portfolios/ayush-folio.md)** — Top-1% portfolio (⭐ 800+)
- **[shubh73/devfolio](04-creative-portfolios/shubh-devfolio.md)** — GSAP starter
- **[Olivier Larose tutorials](04-creative-portfolios/olivier-larose.md)** — Tutorial blog library

### 05 — Immersive 3D (3)
- **[GeethoshGv/React-Three-Fiber](05-immersive-3d/porsche-r3f.md)** — Porsche showroom
- **[anselumjuju/bmw-config](05-immersive-3d/bmw-config.md)** — BMW configurator
- **[14islands/r3f-scroll-rig](05-immersive-3d/r3f-scroll-rig.md)** — DOM↔WebGL sync (⭐ 1.1k+)

### 06 — Editorial scroll (2)
- **[basementstudio/scrollytelling](06-editorial-scroll/basement-scrollytelling.md)** — Declarative scroll API (⭐ 2k+)
- **[btahir/react-kino](06-editorial-scroll/react-kino.md)** — Cinematic primitives

### 07 — YouTube tutorials (4)
- **[MiladiCode/3D-startup-app](07-youtube-tutorials/3d-startup-spline.md)** — HTML+CSS+Spline hero
- **[adrianhajdin/3d-portfolio](07-youtube-tutorials/adrianhajdin-3d-portfolio.md)** — R3F + Framer portfolio
- **[adrianhajdin/threejs-portfolio](07-youtube-tutorials/adrianhajdin-threejs-portfolio.md)** — R3F + GSAP portfolio
- **[Viktor Oddy — AntiGravity](07-youtube-tutorials/viktor-oddy-antigravity.md)** — AI workflow (no code)

### 08 — Web3 / crypto landings (5) 🆕
- **[jagadeesh-k-2802/react-web3-landing-page](08-web3/jagadeesh-react-web3-landing.md)** — Framer + Tailwind Web3
- **[nyxb/cryptoui](08-web3/nyxb-cryptoui.md)** — shadcn-powered DeFi page (⭐ 300+)
- **[0xDigest/nft-landing-page](08-web3/0xdigest-nft-landing.md)** — Lenis + GSAP exact wiring
- **[AdityaAnand1/Crypto-Landing-Page](08-web3/aditya-crypto-landing.md)** — Floating coin hero
- **[PiyushKumar-dev/NFT-Marketplace-Landing-Page](08-web3/piyush-nft-marketplace.md)** — Tilted NFT grid

### 09 — 3D scroll journeys (5) 🆕
- **[designcourse/threejs-webflow](09-3d-scroll-journeys/designcourse-threejs-webflow.md)** — Camera on spline curve
- **[brunosimon/my-room-in-3d](09-3d-scroll-journeys/bruno-simon-my-room.md)** — Baked Blender workflow (⭐ 300+)
- **[pmndrs/react-three-next](09-3d-scroll-journeys/pmndrs-react-three-next.md)** — Next.js 14 + R3F (⭐ 2.9k+)
- **[yomotsu/camera-controls](09-3d-scroll-journeys/yomotsu-camera-controls.md)** — Pro camera damping (⭐ 2.2k+)
- **[yushengdev/scroll-3d-experience](09-3d-scroll-journeys/yushengdev-scroll-3d-experience.md)** — Underwater journey

### 10 — Framer Motion showcase (5) 🆕
- **[framer/motion examples](10-framer-showcase/framer-motion-examples.md)** — Official (⭐ 24k+ parent)
- **[olivierlarose/framer-motion-tutorials](10-framer-showcase/olivierlarose-framer-motion-tutorials.md)** — Narrated recipes (⭐ 700+)
- **[shadcn-ui/ui](10-framer-showcase/shadcn-ui.md)** — Restrained Framer in UI kit (⭐ 75k+)
- **[magicuidesign/magicui](10-framer-showcase/magicui.md)** — 50+ animated components (⭐ 13k+)
- **[aceternity/ui](10-framer-showcase/aceternity-ui.md)** — AI/SaaS aesthetic (⭐ 6k+)

### 11 — Parallax kits (5) 🆕
- **[dixonandmoe/rellax](11-parallax-kits/dixonandmoe-rellax.md)** — Minimal parallax engine (⭐ 7.2k+)
- **[jscottsmith/react-scroll-parallax](11-parallax-kits/react-scroll-parallax.md)** — React parallax at scale (⭐ 1.9k+)
- **[darkroomengineering/lenis](11-parallax-kits/studio-freight-lenis.md)** — Smooth scroll (⭐ 9.8k+)
- **[mkosir/react-parallax-tilt](11-parallax-kits/react-parallax-tilt.md)** — Tilt + glare (⭐ 900+)
- **[keithclark/pure-css-parallax](11-parallax-kits/keithclark-pure-css-parallax.md)** — Zero-JS parallax

### 12 — Three.js art (6) 🆕
- **[pmndrs/drei](12-threejs-art/pmndrs-drei.md)** — Essential R3F primitives (⭐ 8.5k+)
- **[pmndrs/react-postprocessing](12-threejs-art/pmndrs-react-postprocessing.md)** — Bloom/DOF/LUT (⭐ 1k+)
- **[pmndrs/react-three-fiber examples](12-threejs-art/pmndrs-r3f-examples.md)** — Examples index (⭐ 28k+)
- **[pmndrs/react-three-rapier](12-threejs-art/pmndrs-react-three-rapier.md)** — Physics (⭐ 1.3k+)
- **[edankwan/The-Spirit](12-threejs-art/edankwan-the-spirit.md)** — FWA-award GPGPU particles (⭐ 2.3k+)
- **[akella/fake3d](12-threejs-art/akella-fake3d.md)** — Depth-map fake-3D photos (⭐ 500+)

---

## Stack frequency in this hub

```
GSAP (ScrollTrigger)    ████████████████████  30/48 repos
React / Next.js         ███████████████████   45/48 repos
Tailwind CSS            ████████████████      34/48 repos
Three.js / R3F          ██████████████        22/48 repos
Framer Motion           █████████████         18/48 repos
Lenis / Locomotive      ███████               10/48 repos
SplitText               █████                 5/48 repos
shadcn / Radix          ████                  4/48 repos
```

---

## Asset sourcing

Every landing page needs raw material: hero images, 3D models, fonts, audio. The companion
[`ASSETS.md`](ASSETS.md) documents:

- **Part A** — What specific asset sources 9 of the top repos here actually use (Zentry's local-
  only strategy, Bruno Simon's baked Blender workflow, drei's Poly Haven HDRI CDN, Satus's
  Sanity-based pipeline, etc.).
- **Part B** — Non-AI CDNs (Unsplash, Pexels, Poly Haven, Sketchfab, Fontshare, Lucide…).
- **Part C** — **AI image tools**: **Nano Banana** (Gemini 2.5 Flash Image), Midjourney v7,
  Flux, Ideogram 3, Firefly, Recraft, Krea.
- **Part D** — AI video: Runway Gen-4, Kling 2, Pika 2, Luma, Veo 3.
- **Part E** — AI 3D: Meshy, Tripo, Rodin, CSM.
- **Part F** — Depth-map generators (for the `akella/fake3d` technique).
- **Part G** — Recommended asset stack **per landing-page category**.
- **Part H** — License & commercial-safety decision tree.

---

## Workflow: picking repos for a new brief

**1. Brand / product landing?** → Start `01-awwwards-clones/` + `02-agency-sites/`.
**2. Dev / designer portfolio?** → `04-creative-portfolios/` + `07-youtube-tutorials/`.
**3. AI / SaaS / startup landing?** → `10-framer-showcase/` (magicui, aceternity, shadcn).
**4. Web3 / crypto / NFT?** → `08-web3/` + `10-framer-showcase/nyxb-cryptoui`.
**5. Product reveal with 3D?** → `03-apple-product-reveals/` + `05-immersive-3d/`.
**6. Scroll-through-a-world experience?** → `09-3d-scroll-journeys/` + `06-editorial-scroll/`.
**7. Parallax-heavy marketing site?** → `11-parallax-kits/` + `01-awwwards-clones/fullstack-empire-spylt`.
**8. Pure Three.js art piece?** → `12-threejs-art/`.

---

## Contributing (for humans)

- One markdown ficha per repo, named `<org>-<slug>.md`.
- Fields required: **URL**, **Stars (approx)**, **Stack**, **Techniques**, **Why inspiring**.
- Optional: screenshot (`assets/<slug>.webp`, ≤ 300 KB).
- Update this README's Index + Matrix when adding new entries.

## License

This is a curation project — all linked repos retain their own licenses.
Individual fiches are MIT.
