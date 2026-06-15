# University Life — Strategy & Organizational Development

An award-style landing page for NYU's Division of University Life **Strategy and
Organizational Development (SaOD)** team, built with **GSAP** and **Three.js**.

## Highlights
- Three.js hero: a flowing GLSL particle field + slowly rotating wireframe
  icosahedron, with mouse parallax (static frame when `prefers-reduced-motion`)
- Lenis smooth scrolling synced to GSAP ScrollTrigger
- Scroll-reveals, word-by-word mission reveal, animated stat counters, and a
  desktop horizontal-pin gallery for the four areas (stacks vertically on mobile)
- Loader, custom cursor (desktop), animated mobile menu, scroll progress bar
- Fully responsive and mobile-friendly; single-file `index.html`, no build step
- All content sourced from the SaOD mission, area descriptions, and the
  University Life Monthly Brief (Spring 2026 wellbeing data)

## Sections
Hero · Mission · What we provide (6 service lines) · Our areas (4) · Impact ·
Roadmap (Spring 2026) · Connect

## Run locally
```bash
python3 -m http.server 5183 --directory .
# open http://localhost:5183
```

## Deploy
Static site — any host works. For GitHub Pages, enable Pages on `main` (root).
All dependencies (GSAP, ScrollTrigger, Three.js, Lenis) load from HTTPS CDNs.
It also drops cleanly into a Google Sites page via an **Embed → By URL/code**
block if hosted, or as a full-page embed.
