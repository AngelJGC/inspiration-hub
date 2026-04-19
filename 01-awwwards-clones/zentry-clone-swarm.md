# Zentry clone swarm

> **A cluster of community Zentry clones.** Useful for comparing different implementations of the
> same design — each author solved the bento/clip-path/pin pattern differently.

## Repos

| Repo | Notes |
| --- | --- |
| [sahilsingh12221802/Zentry](https://github.com/sahilsingh12221802/Zentry) | Clean Vite+React build, close to SOTM original |
| [33Frok1e/Zentry](https://github.com/33Frok1e/Zentry) | Good README; Tailwind config tuned for the dark palette |
| [freddyfavour/Zentry-Clone](https://github.com/freddyfavour/Zentry-Clone) | Deployed on Netlify; focuses on performance |
| [Evans-Munatsa/Zentry-Clone](https://github.com/Evans-Munatsa/Zentry-Clone) | Simplified version — good for beginners |

## Stack (all share)

- React · Vite · Tailwind · GSAP (ScrollTrigger) · clsx

## Why these matter

If the user wants a **Zentry-style landing** but your first approach breaks on mobile or scrolls
janky, diff these four to see different tile-grid strategies, different scrub values, different
`gsap.matchMedia` breakpoints. The adrianhajdin version is the canonical one — these are the
"how would you do it differently" companions.
