# Inspiration Hub — React · GSAP · Three.js landing pages

> Curated library of high-quality open-source landing pages, portfolios and agency sites.
> Built as a reference for future AI coding sessions (Claude, Cursor, etc.) when the user asks
> for a new landing page and wants it inspired by the best-in-class work on GitHub.

---

## Purpose

When the user asks for a new landing page or marketing site, **start here**. Every entry in this
hub has been vetted for:

- High star count and active maintenance
- Modern stack (React / Next.js / Three.js / GSAP / Framer Motion / Lenis)
- A named, recognisable technique worth stealing (clip-path reveal, scroll-pinned hero, SplitText, etc.)
- A recreatable result — not just a pretty demo, but code you can learn from

This repo was born from the **Obsidiana mezcal redesign** (Apr 2026) where we rebuilt a page in
Zentry/Spylt style by studying the Fullstack-Empire + adrianhajdin award-winning-website repos.
Every subsequent entry here extends that vocabulary.

---

## How to use this repo (for AI agents)

1. Read this README to get the category map.
2. Pick 2–3 repos whose techniques match the brief (e.g. "editorial scroll story" → `06-editorial/`).
3. Read each repo's `.md` ficha in this hub — it captures the stack, standout techniques, and the
   reason the repo matters, so you don't need to clone them unless you want the full source.
4. For full source, clone the URL listed in the ficha.
5. Cross-reference with the **Techniques Matrix** below to avoid duplicating a pattern.

---

## Categories

| #  | Folder                     | Vibe                                      | Best for                                  |
| -- | -------------------------- | ----------------------------------------- | ----------------------------------------- |
| 01 | `01-awwwards-clones/`      | SOTM / SOTD rebuilds                      | Bold kinetic hero, clip-path, scroll-pin  |
| 02 | `02-agency-sites/`         | Studio / agency landings                  | Magnetic cursor, grid hover, transitions  |
| 03 | `03-apple-product-reveals/`| Apple event / iPhone clones               | 3D GLB, scroll-scrubbed camera, variants  |
| 04 | `04-creative-portfolios/`  | Dev + designer portfolios                 | Preloader, project strip, case studies    |
| 05 | `05-immersive-3d/`         | WebGL product + configurators             | R3F, drei, HDRI, shader materials         |
| 06 | `06-editorial-scroll/`     | NYT-style scrollytelling                  | Video scrub, waypoint-driven prose        |
| 07 | `07-youtube-tutorials/`    | Repos from YouTube build-along videos     | Beginner-friendly full builds             |

---

## Techniques Matrix

| Technique                          | Primary reference                               |
| ---------------------------------- | ----------------------------------------------- |
| Zentry-style clip-path reveal      | `01-awwwards-clones/adrianhajdin-award-winning` |
| Spylt kinetic typography           | `01-awwwards-clones/fullstack-empire-spylt`     |
| Video-masked section reveal        | `01-awwwards-clones/adrianhajdin-gta-vi`        |
| SplitText character scrub          | `01-awwwards-clones/adrianhajdin-cocktails`     |
| 3D product variant picker          | `03-apple-product-reveals/adrianhajdin-iphone`  |
| Scroll-pinned horizontal panels    | `01-awwwards-clones/fullstack-empire-spylt`     |
| Magnetic cursor + page transitions | `02-agency-sites/dennis-snellenberg`            |
| DOM↔WebGL sync (hybrid 3D/text)    | `05-immersive-3d/r3f-scroll-rig`                |
| Scrollytelling primitives (React)  | `06-editorial-scroll/basement-scrollytelling`   |
| Scrollytelling primitives (v2)     | `06-editorial-scroll/react-kino`                |
| Car configurator                   | `05-immersive-3d/bmw-config`                    |
| Apple MacBook scroll landing       | `03-apple-product-reveals/adrianhajdin-macbook` |

---

## Index (one-line per repo)

### 01 — Awwwards clones
- **[adrianhajdin/award-winning-website](01-awwwards-clones/adrianhajdin-award-winning.md)** — Zentry SOTM rebuild (⭐ 2.3k+)
- **[adrianhajdin/jsm_gta_vi_landing](01-awwwards-clones/adrianhajdin-gta-vi.md)** — GTA VI trailer landing (⭐ 500+)
- **[adrianhajdin/gsap_cocktails](01-awwwards-clones/adrianhajdin-cocktails.md)** — Beverage brand SplitText reveal (⭐ 300+)
- **[Fullstack-Empire/GSAP-Awwwards-Website](01-awwwards-clones/fullstack-empire-spylt.md)** — Community Spylt/Awwwards rebuild
- **Zentry clone swarm** — `sahilsingh12221802/Zentry`, `33Frok1e/Zentry`, `freddyfavour/Zentry-Clone`, `Evans-Munatsa/Zentry-Clone`

### 02 — Agency / studio sites
- **[Sankalp20Tiwari/spylt](02-agency-sites/sankalp-spylt.md)** — Pixel-honest Tubik Studio "Spylt" rebuild
- **[AliBagheri2079/dennis-snellenberg-portfolio](02-agency-sites/dennis-snellenberg.md)** — Awwwards solo-dev portfolio clone
- **[Shatlyk1011/agency-website](02-agency-sites/shatlyk-agency.md)** — Next.js + Framer agency page
- **[github.com/topics/awwwards-inspired](02-agency-sites/awwwards-inspired-topic.md)** — Ochi / k72-style clones collection

### 03 — Apple-product-style reveals
- **[adrianhajdin/iphone](03-apple-product-reveals/adrianhajdin-iphone.md)** — iPhone 15 Pro R3F experience (⭐ 2k+)
- **[BackBenchDreamer/iphone15-site-clone](03-apple-product-reveals/iphone15-clone.md)** — Lean iPhone clone
- **[adrianhajdin/gsap_macbook_landing](03-apple-product-reveals/adrianhajdin-macbook.md)** — MacBook on-scroll hero

### 04 — Creative portfolios
- **[ayush013/folio](04-creative-portfolios/ayush-folio.md)** — Highly-starred creative dev portfolio (⭐ 800+)
- **[shubh73/devfolio](04-creative-portfolios/shubh-devfolio.md)** — Clean GSAP portfolio starter
- **[Olivier Larose tutorials](04-creative-portfolios/olivier-larose.md)** — Definitive Next.js + Framer Motion tutorial library

### 05 — Immersive 3D
- **[GeethoshGv/React-Three-Fiber (Porsche)](05-immersive-3d/porsche-r3f.md)** — Porsche showroom scene
- **[anselumjuju/bmw-config](05-immersive-3d/bmw-config.md)** — Full BMW configurator
- **[14islands/r3f-scroll-rig](05-immersive-3d/r3f-scroll-rig.md)** — DOM↔WebGL sync (⭐ 1.1k+)

### 06 — Editorial scroll
- **[basementstudio/scrollytelling](06-editorial-scroll/basement-scrollytelling.md)** — Declarative scroll API (⭐ 2k+)
- **[btahir/react-kino](06-editorial-scroll/react-kino.md)** — Cinematic primitives library

### 07 — YouTube tutorials
- **[MiladiCode/3D-startup-app](07-youtube-tutorials/3d-startup-spline.md)** — HTML+CSS+Spline 3D hero
- **[adrianhajdin/3d-portfolio](07-youtube-tutorials/adrianhajdin-3d-portfolio.md)** — R3F + Framer Motion portfolio
- **[adrianhajdin/threejs-portfolio](07-youtube-tutorials/adrianhajdin-threejs-portfolio.md)** — R3F + GSAP portfolio
- **[Viktor Oddy — AntiGravity workflow](07-youtube-tutorials/viktor-oddy-antigravity.md)** — AI-workflow (no code repo)

---

## Stack frequency in this hub

```
GSAP (ScrollTrigger)    ████████████████████  20/24 repos
React / Next.js         ████████████████████  22/24 repos
Tailwind CSS            █████████████████     17/24 repos
Three.js / R3F          ████████████          12/24 repos
Framer Motion           ███████               8/24 repos
Lenis / Locomotive      ██████                6/24 repos
SplitText               █████                 5/24 repos
```

---

## Contributing (for humans)

- One markdown ficha per repo, named `<org>-<slug>.md`.
- Fields required: **URL**, **Stars (approx)**, **Stack**, **Techniques**, **Why inspiring**.
- Optional: screenshot (`assets/<slug>.webp`, ≤ 300 KB).
- Update this README's Index + Matrix when adding new entries.

## License

This is a curation project — all linked repos retain their own licenses.
Individual fiches are MIT.
