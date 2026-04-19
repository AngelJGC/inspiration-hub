# edankwan/The-Spirit

> **FWA-awarded classic.** Still one of the most elegant demonstrations of GPU particle
> rendering on the open web.

- **URL:** https://github.com/edankwan/The-Spirit
- **Live:** http://edankwan.com/experiments/the-spirit/
- **Stars:** ⭐ 2.3k+
- **Stack:** Three.js · WebGL GPGPU

## Techniques

- **GPGPU particle simulation** writing velocities into floating-point textures.
- **Custom ping-pong FBO shader pipeline** — two framebuffers alternating as read/write targets.
- **Motion blur post-effect** — the signature "flowing silk" look.
- **Triangle particles oriented along velocity vectors** — each particle knows where it's going.

## Why inspiring

When you need **"a million particles that flow like fluid"** — this is the reference. The ping-
pong FBO pattern is the foundation of every fluid sim, smoke sim, and particle advection you'll
see on modern Awwwards sites. Older than many repos here (2015), but the technique hasn't aged.

## Cross-refs

- Modern React equivalent: R3F examples with GPGPU (see `pmndrs-r3f-examples`).
