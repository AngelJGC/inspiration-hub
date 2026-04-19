# adrianhajdin/jsm_gta_vi_landing

> **GTA VI trailer-site feel.** Masterclass in video-locked scroll pacing.

- **URL:** https://github.com/adrianhajdin/jsm_gta_vi_landing
- **Stars:** ⭐ 500+ (approx)
- **Stack:** React · Vite · Tailwind · GSAP (ScrollTrigger, ScrollSmoother)

## Techniques worth stealing

- **Pinned cinematic sections** — every section pins for a few viewport-heights, letting the
  background video finish a beat before unpinning.
- **Synced background video** — the `<video>` `currentTime` is driven by
  `ScrollTrigger.scrub`, so scroll position == playhead. Iconic "scroll to play" trick.
- **Parallax foreground + background video** at different rates.
- **Image-mask reveals** — silhouettes cut out of a video layer.

## Why inspiring

If the brief is "make it feel like a blockbuster trailer", this is the reference. The technique
of scrubbing a muted video from scroll is deceptively simple and produces outsized emotional
impact. Works great for product launches, event landings, documentary sites.

## Cross-refs

- Similar video-scrub technique: `02r-milpa` (NYT-style clip-path video frame scrub).
- Compose with: `adrianhajdin-cocktails` (add SplitText over a scrubbed video).
