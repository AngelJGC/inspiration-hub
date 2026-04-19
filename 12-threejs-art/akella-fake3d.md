# akella/fake3d (Yuri Artiukh)

> **The "2D photo that fakes 3D" effect trending across portfolio sites.** Minimal, annotated reference.

- **URL:** https://github.com/akella/fake3d
- **Live (Codrops tutorial):** https://tympanus.net/Tutorials/DepthMapPhotoEffect/
- **Stars:** ⭐ 500+
- **Stack:** Three.js + GLSL · raw WebGL variants

## Techniques

- **Depth-map driven "fake 3D" photo parallax in a fragment shader** — supply the original image
  + a depth map (grayscale), shader offsets each pixel's UV based on depth + pointer position.
- **Pointer UV offset applied per-channel** — optional RGB chromatic split for a "VHS" feel.
- **Shader noise as a displacement mask** — organic rippling motion.
- **Single-quad-plus-shader pattern** — no geometry needed; everything in the fragment shader.

## Why inspiring

This effect is **everywhere in 2024-2026 portfolios** (Landr, Stripe, creative dev sites). One
photo + one depth map + ~60 lines of GLSL = 3D-feeling hero that loads in <200 KB. Way cheaper
than an actual 3D scene, and works on any device.

## How to generate the depth map

- Photoshop's "Neural Filters → Depth Blur" exports a depth map.
- iPhone Portrait mode photos include depth data.
- Runway / DALL·E / SDXL models can generate depth maps from any image.

## Cross-refs

- Next-level version: `r3f-scroll-rig` (05-immersive-3d/) — promote DOM images to full shaders.
