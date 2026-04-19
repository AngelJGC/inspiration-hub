# pmndrs/drei

> **Every "wow" R3F site ships with drei.** Reading its source teaches idiomatic R3F and shader
> material construction.

- **URL:** https://github.com/pmndrs/drei
- **Live:** https://drei.docs.pmnd.rs
- **Stars:** ⭐ 8.5k+
- **Stack:** React Three Fiber

## Essential primitives

- **`MeshTransmissionMaterial`** — realistic glass with caustics (used for bottles, crystals, orbs).
- **`<Environment>` + `<Lightformer>`** — composable studio lighting (soft light, ring-light
  reflections).
- **`<Float>`** — adds gentle bobbing motion to any child mesh.
- **`<ContactShadows>`** — fake ground shadow without a real plane/light.
- **`<Caustics>`** — underwater / translucent scene lighting.
- **`<View>`** — multiple DOM-positioned 3D viewports inside one canvas.

## Why inspiring

If R3F is the engine, drei is the **body kit**. 90% of the visual tricks you see in Awwwards
WebGL work are one-line drei components. Read `MeshTransmissionMaterial.tsx` for the best
glass-in-the-browser shader you'll find.

## Used in this showcase

- `06r-obsidiana` bottle uses `MeshTransmissionMaterial` directly from drei.
- `05r-flora` museum uses `<Environment>` + `<Caustics>`.
