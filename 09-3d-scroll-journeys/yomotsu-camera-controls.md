# yomotsu/camera-controls

> **The camera engine under most "scroll through a 3D world" sites.**

- **URL:** https://github.com/yomotsu/camera-controls
- **Live:** https://yomotsu.github.io/camera-controls/examples/
- **Stars:** ⭐ 2.2k+
- **Stack:** Vanilla Three.js (R3F bindings available via drei)

## Techniques

- **`fitToBox` / `fitToSphere`** for auto-framing meshes during scroll.
- **Smooth damping** on every camera transform (position, target, azimuth, polar).
- **Save/restore camera state** — snapshot at keyframed scroll stages, tween back.
- **Collision detection** with scene colliders — camera can't clip through walls.

## Why inspiring

Not a landing page itself, but this library is **what upgrades a homemade R3F+GSAP scroll scene
from jittery to buttery**. Drop it in and every camera move gets professional damping for free.
The `fitToBox` helper is a lifesaver when you want to auto-frame objects of unknown size.

## Cross-refs

- Paired with: `designcourse/threejs-webflow` (camera curves).
- Used inside: most `pmndrs/drei` examples.
