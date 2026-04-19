# ASSETS — Where the hub repos get their images, 3D, fonts, audio

> **Companion to [`README.md`](README.md).** When you're building a landing page inspired by one
> of the 48 repos in this hub, this document tells you **where to get the raw material** —
> images, videos, 3D models, HDRIs, fonts, audio — and which **AI tools** to reach for when
> hand-sourcing isn't fast enough.

**Answers:** *"Where does Bruno Simon get his baked textures?"* · *"Does Zentry use Unsplash?"*
*"What's Nano Banana and when do I use it?"* · *"How do I make a depth map for the fake3d
shader?"*

---

## Part A — Asset sources found in specific repos

### 01 — Awwwards clones

#### `adrianhajdin/award-winning-website` (Zentry clone)
- **Images:** Local only in `public/img/`. No Unsplash, no CDN.
- **Videos:** Local `.mp4` in `public/videos/` (`hero-1..4.mp4`, `feature-1..5.mp4`, ~1–13 MB each).
  The full asset bundle is a Google Drive zip linked from JSM's README.
- **Fonts:** Custom `.woff2` bundled in `public/fonts/` — `zentry-regular.woff2`,
  `circularweb-book.woff2`, `general.woff2`, `robert-medium.woff2`, `robert-regular.woff2`.
  These mirror Zentry's actual site fonts (educational-use disclaimer).
- **3D:** None (pure GSAP + clip-paths).
- **Takeaway:** **Zero-runtime-asset-dependency**. Everything ships with the repo.

#### `olivierlarose/youtube-tutorials`
- **Images:** Unsplash photos **downloaded and self-hosted** (no `images.unsplash.com` URLs, no
  attribution files). Pattern: `public/images/floating_1.jpg ... floating_8.jpg`, ~70–120 KB.
- **Fonts:** `next/font/google` or local `.woff2`.
- **3D:** drei primitives or single `.glb` re-exported from Sketchfab. The earth tutorial uses
  a NASA Blue Marble JPG.
- **Takeaway:** **Re-source via Unsplash/Pexels before shipping** — he doesn't attribute.

### 02 — Agency sites

#### `darkroomengineering/satus`
- **CMS + image source:** **Sanity** (first-class). Direct deps: `@sanity/asset-utils`,
  `@sanity/image-url`, `next-sanity` v12. All images go through `@/components/ui/image` which
  wraps Sanity's CDN (`cdn.sanity.io`).
- **Secondary (optional scaffold):** Shopify, HubSpot integrations.
- **Fonts:** `public/fonts/` with a config loader. **No Google Fonts**.
- **Banner GIF:** `assets.darkroom.engineering/satus/banner.gif` (their own S3/CF bucket).
- **Takeaway:** If you clone Satus, **plan for a Sanity project** (free tier works). This is
  how agencies scale image pipelines.

### 03 — Apple product reveals

#### `adrianhajdin/iphone`
- **3D:** Single `scene.glb` in `public/models/`. Re-exported from Apple's official iPhone 15
  Pro USDZ (apple.com/shop/buy-iphone). Converted and compressed. **Redistributed in repo**;
  no external host.
- **Textures:** Baked into the GLB.
- **HDRI:** None — scene is lit with `SpotLight` + `AmbientLight`.
- **Takeaway:** Grab the same USDZ from Apple, convert with
  [Reality Converter](https://developer.apple.com/augmented-reality/tools/) or
  [gltf-transform](https://gltf-transform.dev/).

### 05 — Immersive 3D

#### `14islands/r3f-scroll-rig`
- **Demo images:** Dropbox-hosted GIFs (README) + `user-images.githubusercontent.com` screenshots.
- **Sandbox content:** Unsplash direct links + small local JPGs.
- **3D:** None bundled — the library is a DOM→WebGL **bridge**, not an asset library.
- **Takeaway:** Consumer brings their own `<img>` / GLB. This library doesn't care what the
  source is.

### 09 — 3D scroll journeys

#### `brunosimon/my-room-in-3d`
- **3D:** Baked `.glb` self-hosted in `static/assets/` — `roomModel.glb`, `macScreenModel.glb`,
  `pcScreenModel.glb`, `topChairModel.glb`, `coffeeSteamModel.glb`, `elgatoLightModel.glb`,
  `googleHomeLedsModel.glb`, `loupedeckButtonsModel.glb`.
- **Textures:** 3 baked lightmap JPGs (`bakedDay.jpg`, `bakedNight.jpg`, `bakedNeutral.jpg`) +
  `lightMap.jpg` + `googleHomeLedMask.png`. All baked in **Blender** and committed.
- **Videos:** `videoPortfolio.mp4`, `videoStream.mp4` for screen surfaces.
- **Decoders:** `static/draco/` + `static/basis/` (Three.js standard).
- **Takeaway:** **Zero third-party CDN**. Bruno's workflow is Blender bake → commit → ship. If
  you want to replicate this aesthetic, learn Blender baking (Three.js Journey lessons 66–69
  teach this).

### 10 — Framer showcase

#### `magicuidesign/magicui`
- **Assets that ship:** None. Components reference placeholder SVGs. A `showcase/` folder has
  brand logos for the marketing marquee, that's it.
- **Icons:** `lucide-react` + `@radix-ui/react-icons` as peer deps.
- **Takeaway:** **Registry-only** (shadcn-style). Bring your own imagery.

#### `aceternity/ui` (site not fully open-sourced)
- **Images:** Mix of `images.unsplash.com` direct URLs + Aceternity-hosted `assets.aceternity.com`
  (Cloudflare R2) for "3D Card", "Wobble Card", "Macbook Scroll" demos.
- **Icons:** `@tabler/icons-react`, `lucide-react`.
- **Fonts:** Google Fonts (Inter, Geist) via `next/font`.
- **3D:** Mostly **CSS perspective + Framer**. "Globe" uses `cobe` (lightweight WebGL, no model).

### 12 — Three.js art

#### `pmndrs/drei`
- **HDRIs:** `<Environment preset="apartment|city|dawn|forest|lobby|night|park|studio|sunset|warehouse" />`
  are **Poly Haven 1k HDRs** re-hosted in the sister repo
  [`pmndrs/drei-assets`](https://github.com/pmndrs/drei-assets) and served via `raw.githack.com`.
  Source constant in `src/core/useEnvironment.tsx`:
  ```
  CUBEMAP_ROOT = 'https://raw.githack.com/pmndrs/drei-assets/456060a26bbeb8fdf79326f224b6d99b8bcce736/hdri/'
  ```
- **Models:** None bundled in drei itself. Storybook examples (e.g. `suzi`, `office-chair`) also
  live in `drei-assets`.
- **Takeaway:** Poly Haven license is **CC0** → drei can safely re-host. For production, download
  from [polyhaven.com](https://polyhaven.com) and self-host.

---

## Part B — Image & video CDNs (non-AI)

### Free, commercial-safe stock (always first stop)

| Source | Best for | Notes |
| --- | --- | --- |
| [**Unsplash**](https://unsplash.com) | Editorial photos, lifestyle, product | Hotlink `?w=1600&auto=format&fit=crop&q=80`. Unsplash+ tier for exclusive. Used in `06r-obsidiana`. |
| [**Pexels**](https://pexels.com) | Photos + videos | Videos up to 4K, free commercial. |
| [**Pixabay**](https://pixabay.com) | Photos, vectors, music, SFX | Lesser quality but broadest library. |
| [**Mixkit**](https://mixkit.co) | Stock video loops | Clean 4K loops — great for hero backgrounds. |
| [**Coverr**](https://coverr.co) | Hero video loops | Curated for landing-page use. |
| [**Pexels Videos**](https://pexels.com/videos) | Cinematic b-roll | Same CC0 license as photos. |

### 3D models

| Source | License | Use |
| --- | --- | --- |
| [**Sketchfab**](https://sketchfab.com) | Mixed (check per-model) | Huge library, filter by CC-BY / CC0 / Royalty-free. |
| [**Poly Haven**](https://polyhaven.com) | **CC0** | HDRIs, textures, models. The gold standard. |
| [**Quaternius**](https://quaternius.com) | CC0 | Low-poly game/prop sets. |
| [**Kenney Assets**](https://kenney.nl/assets) | CC0 | Stylized game assets, clean topology. |
| [**Ready Player Me**](https://readyplayer.me) | RPM license | Avatar GLB, fast integration. |
| [**Three.js examples**](https://github.com/mrdoob/three.js/tree/master/examples/models) | MIT | Canonical demo models (duck, horse, robot). |

### Fonts

| Source | Notes |
| --- | --- |
| [**Google Fonts**](https://fonts.google.com) | `next/font/google` for zero-CLS loading. Safe bet. |
| [**Fontshare**](https://fontshare.com) | Free commercial display/serif fonts — much more "designer-y" than Google Fonts. **This is what agencies actually use.** |
| [**Adobe Fonts**](https://fonts.adobe.com) | Included with CC. Premium licensing. |
| [**Pangram Pangram**](https://pangrampangram.com) | Modern display fonts, some free. |

### Audio

| Source | Use |
| --- | --- |
| [**Freesound**](https://freesound.org) | SFX, ambience, field recordings. CC-licensed. |
| [**Pixabay Music**](https://pixabay.com/music) | Royalty-free background music. |
| [**Zapsplat**](https://zapsplat.com) | Broad SFX library, free w/ registration. |
| [**Epidemic Sound**](https://epidemicsound.com) | Paid, commercially safe, broad library. |
| [**Artlist**](https://artlist.io) | Paid, top-tier curation. |

### Lottie / SVG animations

| Source | Use |
| --- | --- |
| [**LottieFiles**](https://lottiefiles.com) | JSON Lottie animations — `@lottiefiles/react-lottie-player`. |
| [**IconScout**](https://iconscout.com) | Lotties + 3D icons. Paid. |
| [**Rive**](https://rive.app) | Interactive vector animations — tiny `.riv` files. |

### Icons

| Source | Notes |
| --- | --- |
| [**Lucide**](https://lucide.dev) | The shadcn default. 1400+ icons. |
| [**Heroicons**](https://heroicons.com) | By Tailwind team. |
| [**Tabler Icons**](https://tabler-icons.io) | 4900+ icons, used by aceternity. |
| [**Radix Icons**](https://www.radix-ui.com/icons) | Minimal, UI-focused. |
| [**Phosphor Icons**](https://phosphoricons.com) | 6 weights × 9000 icons. |

---

## Part C — AI image generation

> TL;DR: **Nano Banana** for edits + character consistency. **Midjourney v7** for aesthetic
> hero shots. **Flux Pro** for photoreal. **Ideogram 3** when text must render inside the image.
> **Recraft v3** for logos/vectors. **Firefly 3** when the client requires commercial indemnity.

### 🍌 Nano Banana (Google Gemini 2.5 Flash Image) — Aug 2025
- **Strength:** **Character/object consistency across shots** + natural-language local edits
  ("blur background", "remove person", "change jacket to leather"). 10 aspect ratios.
  Invisible SynthID watermark.
- **Why it matters for landing pages:** When you need the **same hero model/product in
  5 different scenes**, Nano Banana is the only model that holds the identity. Perfect for
  multi-section stories where a character recurs.
- **Access:** Gemini API · Google AI Studio · Vertex AI.
- **Pricing:** ~$0.039/image ($30/M output tokens, 1290 tokens/img). Free tier in AI Studio.
- **When to use:** Editing existing photos · character consistency · multi-shot storyboards.

### Midjourney v7 — Apr 2025 (default since Jun 2025)
- **Strength:** Cinematic, richly textured hero imagery. 40% fewer anatomical errors, 35%
  better prompt adherence than v6. New **Draft Mode**, **Omni Reference**, text-to-video.
- **Why it matters:** Nothing else hits the same aesthetic ceiling. If the brief is "luxury
  brand hero" or "editorial cover", Midjourney wins.
- **Pricing:** Basic $10, Standard $30, Pro $60, Mega $120/mo (-20% annual). **No free tier.**
- **When to use:** Hero shots · mood boards · aesthetic reference.

### Flux.1 (Schnell / Dev / Pro) — Black Forest Labs
- **Schnell:** Apache 2.0, fully commercial, 1–4 step distilled. Great for self-hosting or
  real-time tools (Krea).
- **Dev:** Non-commercial weights on Hugging Face, best open-weights quality.
- **Pro / 1.1 Pro / Ultra:** API-only via `bfl.ai`, fal, Replicate. ~$0.04–0.05/image.
- **Why it matters:** Top-tier **photorealism** and prompt fidelity. The workhorse behind many
  indie landing-page hero generators.
- **When to use:** Photoreal product renders · batch generation · self-hosting.

### Ideogram 3.0 — Mar 2025
- **Strength:** Best-in-class **in-image text rendering**. Multi-line posters, Latin, Chinese,
  Arabic, Devanagari all render legibly.
- **Why it matters:** Posters, billboards, magazine covers, typographic heroes — anywhere text
  has to be inside the render.
- **Pricing:** Free daily generations; paid from ~$8/mo.
- **When to use:** Typographic heroes · event posters · brand mockups with signage.

### Adobe Firefly Image 3 / 4 / 5 (currently shipping)
- **Strength:** **Commercial-safe** (trained on licensed Adobe Stock + public domain). IP
  indemnification. Structure Reference, Style Reference, Generative Expand.
- **Why it matters:** **Client work.** When the user is a brand that can't afford IP risk,
  Firefly is the safe choice.
- **Pricing:** Included with Creative Cloud ($22.99+/mo) or standalone Firefly plans.
- **When to use:** Regulated industries · enterprise clients · legal indemnity requirements.

### Recraft v3 — late 2024 (still SOTA for design in 2026)
- **Strength:** The **only** major model generating **true vector (SVG) output** and precise
  typographic placement.
- **Why it matters:** Logos, brand marks, icons, illustrated UI, scalable assets.
- **Pricing:** 50 daily credits free; paid from $10/mo; API $0.04 raster / $0.08 vector.
- **When to use:** Logos · icon sets · illustrated mascots · scalable brand art.

### Krea AI (real-time, multi-model)
- **Strength:** **Real-time canvas** (<50 ms sketch-to-image). Multi-model backend: Flux,
  SDXL, Ideogram, Recraft.
- **Why it matters:** **Rapid iteration** — sketch, drag, re-roll in seconds. Best for mood-
  boarding hero concepts live with a client.
- **Pricing:** 100 free daily units · Basic $9 · Pro $35 · Max $105. Commercial from Basic.
- **When to use:** Mood boarding · live client sessions · exploratory phase.

---

## Part D — AI video generation

### Runway Gen-4 / 4.5 — Mar 2025 / Nov 2025
- **Strength:** Industry benchmark for **character + scene consistency** and realistic physics.
  10 s @ 24 fps, 720p default, upscale to 4K.
- **Use for landings:** Scroll-driven cinematic loops, hero video backgrounds.
- **Pricing:** Free limited trial · Standard $15 · Pro $35 · Unlimited $95.

### Kling 2.0 / 2.1 / 2.5 / 2.6 — Kuaishou
- **Strength:** Excellent **image-to-video** and motion physics. Up to 1080p, 2-minute clips,
  strong character lock.
- **Pricing:** 66 free credits/day · Standard $10 · Pro $25.99 · Premier $64.99.

### Pika 2.0 — Feb 2025
- **Strength:** **Scene Ingredients** — upload your own characters, props, and effects (snow,
  lens flare, film grain) with intensity sliders.
- **Use for landings:** Playful, stylized hero video. Ad-friendly motion.
- **Pricing:** Standard $10/mo (non-commercial) · Pro $35 (commercial + no watermark).

### Luma Dream Machine
- **Strength:** **Keyframes + extend** for longer, continuous shots and animating stills.
- **Use for landings:** Animated still photos (portrait → subtle motion hero).
- **Pricing:** Free · Lite $9.99 · Standard $29.99 (commercial) · Plus $64.99 · Pro $99.99.

### Google Veo 3 / 3.1 — May / Oct 2025
- **Strength:** Native **synchronized audio** (SFX, ambient, lip-synced dialogue). 1080p, 9:16
  vertical, multimodal storyboard→video.
- **Use for landings:** Social-first verticals, short-form teaser reels.
- **Pricing:** API $0.15/s Fast · $0.40/s Standard. Consumer via Google AI Pro $19.99 or
  Ultra $249.99.

---

## Part E — AI 3D generation

### Meshy v4 / v5 / v6
- **Output:** PBR-textured 3D in ~60 s. Exports GLB, FBX, OBJ, USDZ, STL, BLEND.
- **Modes:** A/T-pose for rigging, Low-Poly for games.
- **Pricing:** 200 free initial + 100/mo · Pro $16/mo (annual) · Max $48 · Max Unlimited $96.
  20 credits/generation.
- **Use for landings:** Prop generation for product reveal scenes.

### Tripo 3D
- **Strength:** **Quad topology + auto-rigging** — clean meshes suitable for R3F, not disposable
  scan-style blobs.
- **Pricing:** ~$12/mo for 200 credits.
- **Use for landings:** Hero props that must be animated or rigged.

### Rodin / Hyper3D (Deemos)
- **Strength:** Highest fidelity — **4K PBR textures**, photorealistic, fastest inference among
  premium tiers.
- **Pricing:** from $99/mo.
- **Use for landings:** Single hero prop that must hold up under close camera.

### CSM (Common Sense Machines)
- **URL:** https://3d.csm.ai
- **Strength:** Image/sketch/text → production 3D with **multi-view reconstruction**, PBR, AI
  retexture, text-to-4D, animation library. Unity/Unreal-ready.
- **Pricing:** 10 free credits · Maker 100/mo · Creative Pro 400/mo · Enterprise custom.
- **Use for landings:** Sketch-to-product workflows, rapid prototyping.

---

## Part F — Depth maps (for the `akella/fake3d` technique in `12-threejs-art/`)

The "2D photo that fakes 3D" shader in `akella/fake3d` requires a **grayscale depth map**
alongside the original image. Three ways to produce one in 2026:

### DepthAnything V2 — Hugging Face (current SOTA, 2026)
- **URL:** https://depth-anything.github.io
- **Why:** ViT-L beats MiDaS v3.1 (AbsRel 0.074 vs 0.083). Best single choice for fake3d.
- **How to run:**
  - **In-browser (easiest):** `transformers.js` or WebGPU port.
  - **API:** Replicate, Hugging Face Inference.
  - **Local:** Python + ONNX for batch.

### MiDaS (Intel ISL)
- **URL:** https://github.com/isl-org/MiDaS
- **Why:** Simpler, lighter. PyTorch Hub one-liner.
- **When:** Fallback when DepthAnything is too heavy.

### iPhone Portrait Mode (built-in, free, instant)
- **How:** Any iPhone with dual/LiDAR camera produces a hardware depth channel in Portrait
  photos. Extract via `AVDepthData` (iOS) or HEIC → auxiliary depth map.
- **Why:** Zero cost, metric depth, perfect for **photos the designer shoots themselves**.
- **When:** Designer has access to an iPhone and the hero subject is physically shootable.

---

## Part G — Recommended asset stack by landing-page category

| Category | Image | Video | 3D | Audio | Font |
| --- | --- | --- | --- | --- | --- |
| **01 Awwwards clone** | Unsplash + Midjourney v7 hero | Mixkit loop + Runway Gen-4 | — | Freesound score | Fontshare display |
| **02 Agency site** | Client photos + Flux Pro + Firefly (safe) | Runway Gen-4 | — | Epidemic Sound | Fontshare / Pangram |
| **03 Apple product reveal** | Product photography | Hero loop (Runway/Kling) | Apple USDZ or Meshy | Subtle SFX (Freesound) | Geist / Inter |
| **04 Creative portfolio** | Unsplash + own work | — | Optional R3F scene | — | Fontshare display |
| **05 Immersive 3D** | — | — | Sketchfab + Poly Haven HDRI + Meshy/Rodin | Ambient bed (Pixabay) | Geist Mono for overlay |
| **06 Editorial scroll** | Own photography + Nano Banana edits | Archival / Runway | — | Field recordings (Freesound) | Editorial serif (Fontshare) |
| **07 YouTube tutorial** | Unsplash / Pexels | — | drei primitives | — | Google Fonts |
| **08 Web3 / NFT** | Flux Pro + Ideogram 3 (text-in-image) | Pika 2 for dynamic banners | Meshy props | Synthwave loops (Pixabay) | Monospace (Geist/IBM Plex) |
| **09 3D scroll journey** | — | — | Bruno Simon–style Blender bake + Poly Haven HDRI | Ambient drone | — |
| **10 Framer showcase (AI/SaaS)** | aceternity + Unsplash | Short demo screencaps | — | Minimal SFX | Geist / Inter |
| **11 Parallax** | Nano Banana edits + Krea for iteration | Stock loops | — | — | Display serif |
| **12 Three.js art** | — | — | Generated (Rodin) or hand-authored | Generative ambient | — |

---

## Part H — Licenses & commercial safety

### Traffic-light system

| License | Meaning | Commercial use |
| --- | --- | --- |
| 🟢 **CC0 / Public Domain** | No attribution required. Poly Haven, Kenney, Unsplash, Pexels, Pixabay. | **Safe, no credit needed.** |
| 🟢 **MIT / Apache** | Open-source code licenses; asset usage varies. | Usually safe — read each repo. |
| 🟡 **CC-BY** | Attribution required. Some Freesound, some Sketchfab. | Safe **if** you credit the author. |
| 🟡 **Unsplash License** | Free use, no attribution required, but **can't resell as stock**. | Safe for landings. |
| 🔴 **CC-BY-NC** | Non-commercial only. | **Don't use on client work.** |
| 🔴 **"Editorial only"** | Getty / Shutterstock editorial tiers. | **Don't use in marketing.** |
| 🟢 **Adobe Firefly IP Indemnity** | Adobe pays legal fees if output is challenged. | **Enterprise-grade safe.** |
| 🟡 **Midjourney / Flux / most AI** | You own output on paid tiers; training data is contested. | Safe for most work; **avoid for regulated industries**. |
| 🔴 **Midjourney free / trial** | Output is **not** commercially licensed. | Never ship. |

### Quick decision tree

1. **Client in healthcare / finance / legal / gov?** → Adobe Firefly only.
2. **Client is a startup / agency brand?** → Midjourney, Flux Pro, Ideogram all fine.
3. **Open-source / personal project?** → Anything, credit where required.
4. **Pulling from Sketchfab?** → Filter to CC0 or CC-BY. Check each model's license page.
5. **Photos of real people?** → Unsplash model-released tier, or your own shoots with release forms.

### SynthID note

Google's Nano Banana outputs are watermarked with **SynthID** (invisible, machine-detectable).
This is fine for commercial use but disclose when the context demands (journalism, evidence,
legal).

---

## Asset acquisition checklist for a new landing page

1. **Mood board first** — Krea AI (real-time) or Midjourney Draft Mode.
2. **Lock the hero image** — Midjourney v7 or Flux Pro (for photoreal).
3. **Edit + variations** — Nano Banana for consistent character across sections.
4. **Typographic elements** — Ideogram 3 if text lives inside images; Recraft for logos/vectors.
5. **3D hero prop (if needed)** — Meshy / Rodin / Tripo (pick by fidelity tier).
6. **HDRI lighting** — Poly Haven (CC0) → self-host in `/public/hdri/`.
7. **Background video** — Mixkit / Coverr for stock; Runway Gen-4 / Kling for custom.
8. **Ambient audio** — Pixabay Music / Epidemic Sound.
9. **Icons + UI glyphs** — Lucide / Tabler / Phosphor.
10. **Fonts** — Fontshare for display, Geist/Inter for body.
11. **Optimize** — `sharp` (Next.js built-in), `squoosh.app`, `gltf-transform` for GLB,
    `ffmpeg` for video.
12. **License audit** — confirm every asset against Part H table before shipping.

---

## Related files

- [`README.md`](README.md) — main hub index.
- Per-repo fichas — each notes specific asset paths and sources where known.
