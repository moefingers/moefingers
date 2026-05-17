<div align="center">

<!--
  Hero banner — rotating 50-point sphere + wireframe icosahedron on the
  left, live GitHub + nitrotype stats on the right.
  Source: github.com/moefingers/dynimage  ·  Card type: `hero`
-->
<img alt="moefingers — orbit + GitHub + nitrotype hero banner"
     src="https://dynimage.vercel.app/api/moefingers/hero.svg?nt=bigmoemoney"
     width="100%">

<sub>Sphere + icosahedron · last-year commits · public repos · contribution streak · average WPM · peak WPM · lifetime races · all live</sub>

---

### [Visit my new site — infinite-syndicate.com](https://infinite-syndicate.com)

<a href="https://infinite-syndicate.com">
  <img alt="Infinite Syndicate — a suite of services brought together"
       src="https://dynimage.vercel.app/api/moefingers/syndicate.svg"
       width="100%">
</a>

</div>

---

## The orbit, in four moods

Same sphere + icosahedron, four palette variants. The basic and mono variants adapt to the viewer's GitHub theme via `prefers-color-scheme`; neon and prism layer a continuous hue-rotate so the colors drift forever.

<p align="center">
  <img alt="orbit · basic"
       src="https://dynimage.vercel.app/api/moefingers/orbit.svg?v=basic"
       width="48%">
  <img alt="orbit · prism"
       src="https://dynimage.vercel.app/api/moefingers/orbit.svg?v=prism"
       width="48%">
</p>
<p align="center">
  <img alt="orbit · neon"
       src="https://dynimage.vercel.app/api/moefingers/orbit.svg?v=neon"
       width="48%">
  <img alt="orbit · mono"
       src="https://dynimage.vercel.app/api/moefingers/orbit.svg?v=mono&theme=ocean"
       width="48%">
</p>

---

## Live stats — typing & commits

<p align="center">
  <img alt="Nitrotype typing speed for @bigmoemoney"
       src="https://dynimage.vercel.app/api/bigmoemoney/typing.svg"
       width="58%" align="top">
  <img alt="Compact commits + icosahedron nucleus"
       src="https://dynimage.vercel.app/api/moefingers/nucleus.svg?w=340&h=220"
       width="38%" align="top">
</p>

<img alt="moefingers stats strip — commits, repos, streak, followers"
     src="https://dynimage.vercel.app/api/moefingers/strip.svg"
     width="100%">

<img alt="moefingers prism banner"
     src="https://dynimage.vercel.app/api/moefingers/prism.svg"
     width="100%">

---

## What's powering this README

Every banner is served by [**dynimage**](https://github.com/moefingers/dynimage) — a Next.js edge service that hands back animated SVGs, theme-aware and live-data-driven, that GitHub's `camo` image proxy passes through faithfully. No client JS. The animations run via SMIL + CSS keyframes inside the SVG.

- **`hero` / `orbit` / `nucleus`** — sphere math ported from the [`unlv-museum`](https://github.com/moefingers/unlv-museum) banner-experiments lab: Fibonacci-distributed points, baked rotation keyframes, depth-faded opacity, no real 3D transforms required.
- **`typing`** — live WPM via [**nitrotype-api**](https://github.com/moefingers/nitrotype-api), a tiny proxy that scrapes the `RACER_INFO` blob from nitrotype.com profile pages.
- **`syndicate`** — branded CTA matching the live homepage at [infinite-syndicate.com](https://infinite-syndicate.com).
- **`commits` / `strip` / `prism`** — GitHub GraphQL via `@octokit/graphql` with Next's `fetch` cache.

### Recent

- **Nov 2025** — bypassed nitrotype's Cloudflare gate via browser-style headers in the proxy. The only reason any of this scrape-and-serve existed was that nitrotype refused to expose an API or keys.
- **Now** — animated SVG banner family built on top of the unlv-museum sphere-math experiments. The card abstraction in dynimage made adding seven new live preset banners a single-file-per-banner change.

### Original embeds, kept for posterity

[![Typing race stats — canvas-rendered PNG, original implementation](https://nitrotype-api.vercel.app/api/image-gen/racer-stats/bigmoemoney)](https://nitrotype-api.vercel.app)

[![Fibonacci circles experiment from unlv-museum](https://unlv-museum.infinite-syndicate.com/banner-experiments/12-fibonacci-circles-100.svg)](https://unlv-museum.infinite-syndicate.com)

---

<div align="center">
<sub>Banner cards: <a href="https://github.com/moefingers/dynimage">dynimage</a> · Typing API: <a href="https://github.com/moefingers/nitrotype-api">nitrotype-api</a> · Sphere math: <a href="https://github.com/moefingers/unlv-museum">unlv-museum</a> · Site: <a href="https://infinite-syndicate.com">infinite-syndicate.com</a></sub>
</div>
