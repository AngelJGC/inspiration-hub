# pmndrs/react-three-rapier

> **The cleanest React entry point to Rapier physics** — and the fastest way to ship a physics
> playground page.

- **URL:** https://github.com/pmndrs/react-three-rapier
- **Live:** https://react-three-rapier.pmnd.rs
- **Stars:** ⭐ 1.3k+
- **Stack:** R3F · Rapier physics (WASM)

## Techniques

- **Declarative `<RigidBody>` / `<CuboidCollider>` JSX** — no imperative physics setup.
- **Impulse / force hooks on pointer events** — "click → push" with one line.
- **Instanced rigid bodies for thousands of objects** — confetti, marbles, dominos scale well.
- **Joint / constraint examples** — rope, hinge, distance constraints.

## Why inspiring

Rapier is the **successor to cannon.js** for serious physics on the web. This React binding
makes it absurdly easy to ship an interactive physics scene: click to drop cubes, throw
objects, simulate cloth. Any SaaS landing that wants a "playful hero" sandboxes here.

## Use cases

- Interactive hero (confetti cannon, toy physics).
- Product-playground (stack boxes, knock down tower).
- Onboarding game-ification.

## Cross-refs

- Canvas host: `pmndrs/react-three-fiber`.
- Combine with: `pmndrs/react-postprocessing` for bloom/DOF polish.
