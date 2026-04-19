# anselumjuju/bmw-config

> **Full product-configurator UX — closer to a real automotive brand site.**

- **URL:** https://github.com/anselumjuju/bmw-config
- **Stack:** React Three Fiber · drei · Draco loader

## Techniques worth stealing

- **Full BMW configurator** — body color, wheels, interior swap on a single GLB.
- **Draco-compressed meshes** — aggressive geometry compression for fast loads.
- **Material swap without re-rendering the model** — store materials in a ref, swap per selection.
- **Optimized GLB streaming** — progressive loading with a fallback placeholder.
- **UI driven by Zustand store** — clean decoupling between UI and 3D state.

## Why inspiring

This is how **real automotive/e-commerce 3D configurators** are built. If the brief is
"customizable product" (shoe, car, furniture, jewelry), this repo has the full pattern.

## Cross-refs

- Lighter version: `porsche-r3f` (no configurator, just showcase).
- UI inspiration: `adrianhajdin-iphone` (product reveal with variant picker).
