# brunosimon/my-room-in-3d

> **Bruno Simon's own room.** Still the reference for baked-texture, web-scale 3D scenes.

- **URL:** https://github.com/brunosimon/my-room-in-3d
- **Live:** https://my-room-in-3d.bruno-simon.com
- **Stars:** ⭐ 300+
- **Stack:** Three.js · Webpack · Howler

## Techniques

- **Baked lighting workflow** — Blender bake → single texture → unlit `MeshBasicMaterial`.
  This is how you ship "photoreal" scenes that load in <2s.
- **Per-mesh video textures** — TV/monitor screens play looping videos as materials.
- **Custom shader material** for animated neon/LED edges.
- **Fireflies particle system** with custom shader.

## Why inspiring

Bruno teaches Three.js Journey (the course). This is his portfolio-scale demo. **The baked
texture trick** — pre-computing all lighting in Blender and shipping the result as a single
image — is how you get visuals way above your polygon budget. Every "miniature world" site
built in 2020-2026 uses this workflow.

## Cross-refs

- Tutorial form: https://threejs-journey.com
- Scroll integration: `designcourse/threejs-webflow`, `pmndrs/react-three-next`.
