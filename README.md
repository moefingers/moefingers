<div align="center">

<!--
  Hero — rotating sphere + icosahedron on the left, all-stats panel on
  the right (commits · repos · streak · avg/peak WPM · races).
-->
<img alt="moefingers — orbit + GitHub + nitrotype hero banner"
     src="https://dynimage.vercel.app/api/moefingers/hero.svg?nt=bigmoemoney"
     width="100%">

<sub>Sphere + icosahedron · last-year commits · public repos · contribution streak · average WPM · peak WPM · lifetime races · all live</sub>

---

### [Visit my new site — infinite-syndicate.com](https://infinite-syndicate.com)

<a href="https://infinite-syndicate.com">
  <img alt="Infinite Syndicate — counter-rotating sacred-geometry lattice (lifted directly from the live homepage) over Software · Computers · Client Portal"
       src="https://dynimage.vercel.app/api/moefingers/syndicate.svg"
       width="100%">
</a>

<sub>The lattice pattern is the brand watermark from infinite-syndicate.com — two layers counter-rotate while breathing in and out at offset phases.</sub>

</div>

---

## Side by side — GitHub commits, typing speed

Two wide compound banners with mirrored layouts: prism-orbit on the left side of the commits card, neon-orbit on the right side of the typing card. Same sphere geometry, two different palettes, paired so the eye moves across them.

<img alt="@moefingers — last-year GitHub commits with prism sphere"
     src="https://dynimage.vercel.app/api/moefingers/commits-orbit.svg"
     width="100%">

<img alt="@bigmoemoney typing speed — nitrotype WPM with neon sphere"
     src="https://dynimage.vercel.app/api/bigmoemoney/typing-orbit.svg"
     width="100%">

---

## The orbit, on its own

Same sphere + icosahedron, four palette variants. Basic and mono adapt to the viewer's GitHub theme via `prefers-color-scheme`; neon and prism layer a continuous hue-rotate so the colors drift forever.

<p align="center">
  <img alt="orbit · basic" src="https://dynimage.vercel.app/api/moefingers/orbit.svg?v=basic"  width="48%">
  <img alt="orbit · prism" src="https://dynimage.vercel.app/api/moefingers/orbit.svg?v=prism"  width="48%">
</p>
<p align="center">
  <img alt="orbit · neon"  src="https://dynimage.vercel.app/api/moefingers/orbit.svg?v=neon"   width="48%">
  <img alt="orbit · mono"  src="https://dynimage.vercel.app/api/moefingers/orbit.svg?v=mono&theme=ocean" width="48%">
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

- **`hero` / `orbit` / `commits-orbit` / `typing-orbit` / `nucleus`** — sphere + icosahedron math ported from the [`unlv-museum`](https://github.com/moefingers/unlv-museum) banner-experiments lab. Fibonacci-distributed points + baked rotation keyframes + depth-faded opacity. No real 3D transforms required.
- **`typing` / `typing-orbit`** — live WPM via [**nitrotype-api**](https://github.com/moefingers/nitrotype-api), a tiny proxy that scrapes the `RACER_INFO` blob off nitrotype.com profile pages.
- **`syndicate`** — Branded CTA built around the actual sacred-geometry lattice from [infinite-syndicate.com](https://infinite-syndicate.com)'s homepage; two layers counter-rotate while breathing in and out on offset phases.
- **`commits` / `strip` / `prism`** — GitHub GraphQL via `@octokit/graphql` with Next's `fetch` cache.

### Recent

- **Now** — `commits-orbit` and `typing-orbit` shipped: paired wide banners with sphere visuals on opposite sides for a left/right diptych. Syndicate rebuilt around the live brand lattice (`/public/radial1.svg`) with counter-phased shrink/expand animation.
- **Nov 2025** — bypassed nitrotype's Cloudflare gate via browser-style headers in the proxy. The only reason any of this scrape-and-serve existed was that nitrotype refused to expose an API or keys.

### Original embeds, kept for posterity

[![Typing race stats — canvas-rendered PNG, original implementation](https://nitrotype-api.vercel.app/api/image-gen/racer-stats/bigmoemoney)](https://nitrotype-api.vercel.app)

[![Fibonacci circles experiment from unlv-museum](https://unlv-museum.infinite-syndicate.com/banner-experiments/12-fibonacci-circles-100.svg)](https://unlv-museum.infinite-syndicate.com)

---

<div align="center">
<sub>Banner cards: <a href="https://github.com/moefingers/dynimage">dynimage</a> · Typing API: <a href="https://github.com/moefingers/nitrotype-api">nitrotype-api</a> · Sphere math: <a href="https://github.com/moefingers/unlv-museum">unlv-museum</a> · Site: <a href="https://infinite-syndicate.com">infinite-syndicate.com</a></sub>
</div>
