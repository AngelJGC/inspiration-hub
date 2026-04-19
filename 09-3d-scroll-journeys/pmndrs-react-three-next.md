# pmndrs/react-three-next

> **Official pmndrs answer to "how do I do Three.js in Next 14".** Solves the route-level canvas
> problem most tutorials duck.

- **URL:** https://github.com/pmndrs/react-three-next
- **Live:** https://react-three-next.vercel.app
- **Stars:** ⭐ 2.9k+
- **Stack:** Next.js 14 App Router · React Three Fiber · drei · Tailwind

## Techniques

- **Shared WebGL canvas across routes** via **tunnel-rat** pattern — canvas doesn't re-mount
  between pages; 3D state persists across navigations.
- **DOM-synced 3D views** using drei `<View>` — multiple 3D viewports inside a single canvas,
  positioned by DOM refs.
- **SSR-safe dynamic imports** with `ssr: false`.
- **Scroll-driven camera** via drei `<ScrollControls>` + `useScroll`.

## Why inspiring

This is the **canonical template** if you're building a Next.js + R3F site. The tunnel-rat
trick alone saves you from the dreaded "canvas flashes on route change" bug. Read the layout
and copy the provider setup — you'll save a full day.

## Cross-refs

- Related R3F utilities: `pmndrs/drei` (12-threejs-art/).
- Scroll journeys: `designcourse/threejs-webflow`.
