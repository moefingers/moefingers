<!--
  Two compound banners up top — GitHub and Nitrotype, each with their
  own brand mark sitting inside the icosahedron and the orbit on the
  opposite side from the data panel.
-->

<img alt="@moefingers — last-year GitHub commits, neon-palette sphere with GitHub octocat at icosahedron center"
     src="https://dynimage.vercel.app/api/moefingers/commits-orbit.svg"
     width="100%">

<img alt="@bigmoemoney typing speed — nitrotype WPM, prism-palette sphere with Nitrotype N at icosahedron center"
     src="https://dynimage.vercel.app/api/bigmoemoney/typing-orbit.svg"
     width="100%">

<div align="center">

### [Visit my new site — infinite-syndicate.com](https://infinite-syndicate.com)

<a href="https://infinite-syndicate.com">
  <img alt="Infinite Syndicate — counter-rotating sacred-geometry lattice (lifted directly from the live homepage) over Software · Computers · Client Portal"
       src="https://dynimage.vercel.app/api/moefingers/syndicate.svg"
       width="100%">
</a>

<sub>The lattice is the brand watermark from infinite-syndicate.com — two layers counter-rotate while breathing in and out at offset phases, each scaling around its own center so they flow through each other.</sub>

</div>

---

## The orbit, on its own

Same sphere + icosahedron in two palettes — prism (warm amber icosa over rainbow dots) and neon (cyan icosa over a magenta-to-cyan band). Both layer a continuous hue-rotate so the colors drift forever; both adapt the wireframe + label colors to the viewer's GitHub theme via `prefers-color-scheme`.

<p align="center">
  <img alt="orbit · prism" src="https://dynimage.vercel.app/api/moefingers/orbit.svg?v=prism" width="48%">
  <img alt="orbit · neon"  src="https://dynimage.vercel.app/api/moefingers/orbit.svg?v=neon"  width="48%">
</p>

---

## Quick stats — the rest of the family

<img alt="moefingers stats strip — commits, repos, streak, followers"
     src="https://dynimage.vercel.app/api/moefingers/strip.svg"
     width="100%">

<img alt="moefingers prism color-band banner"
     src="https://dynimage.vercel.app/api/moefingers/prism.svg"
     width="100%">

---

## What's powering this README

Every banner is served by [**dynimage**](https://github.com/moefingers/dynimage) — a Next.js edge service that returns animated SVGs, theme-aware and live-data-driven, that GitHub's `camo` image proxy passes through faithfully. No client JS; animations run via SMIL + CSS keyframes inside the SVG.

- **`commits-orbit` / `typing-orbit` / `orbit`** — sphere + icosahedron math ported from the [`unlv-museum`](https://github.com/moefingers/unlv-museum) banner-experiments lab. Fibonacci-distributed points + baked rotation keyframes + depth-faded opacity. No real 3D transforms required. The platform brand mark sits at the icosa's geometric center, behind the wireframe; the rotating geometry spins around it.
- **`typing-orbit`** — live WPM via [**nitrotype-api**](https://github.com/moefingers/nitrotype-api), a tiny proxy that scrapes the `RACER_INFO` blob off nitrotype.com profile pages.
- **`syndicate`** — Branded CTA built around the actual sacred-geometry lattice from [infinite-syndicate.com](https://infinite-syndicate.com)'s homepage; two layers counter-rotate while breathing in and out on offset phases (each scaling around its own center so the patterns pass through one another).
- **`commits-orbit` / `strip` / `prism`** — GitHub GraphQL via `@octokit/graphql` with Next's `fetch` cache.

### Recent

- **Now** — brand marks (GitHub octocat + Nitrotype N) inlined at the icosa center on the two compound cards. Syndicate lattice fixed so the scale animation pivots locally instead of drifting toward the banner top-left.
- **Last week** — `commits-orbit` and `typing-orbit` shipped: paired wide banners with sphere visuals on opposite sides for a left/right diptych.
- **Nov 2025** — bypassed nitrotype's Cloudflare gate via browser-style headers in the proxy. The only reason any of this scrape-and-serve existed was that nitrotype refused to expose an API or keys.

---

<div align="center">
<sub>Banner cards: <a href="https://github.com/moefingers/dynimage">dynimage</a> · Typing API: <a href="https://github.com/moefingers/nitrotype-api">nitrotype-api</a> · Sphere math: <a href="https://github.com/moefingers/unlv-museum">unlv-museum</a> · Site: <a href="https://infinite-syndicate.com">infinite-syndicate.com</a></sub>
</div>
