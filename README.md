# MekaVerse

A cinematic web3 game portal built in **Astro**, styled entirely from the **MekaVerse design system** — a "monochrome gallery for digital artifacts": pure-black void, white ink type, a single charcoal control, hairline frost borders, and full-bleed rendered artwork carrying all the color.

## Design system fidelity

- **Palette** — Void `#000000`, Bone `#ffffff`, Charcoal `#444345`, Frost `#e2e2e2`, Ash `#b8bab9`. No chromatic accent anywhere; all color comes from the imagery.
- **Type** — Inter at weight 400 for display (substitute for Roobert), stacked at extreme sizes with `line-height: 0.78`; JetBrains Mono 10–12px at `-0.02em` for all chrome (substitute for GT America Mono).
- **Signature underline mark** — a 1px Frost hairline beneath each line of every stacked display title, extending to 30–58% of the line width. Animates in on scroll.
- **Surfaces & elevation** — flat. No shadows anywhere; elevation is the Void → Charcoal → Ash stack plus hairline borders.
- **Radii** — the 2 / 10 / 20 triad only (buttons 2px, cards 10px, containers 20px).
- **Layout** — full-bleed cinematic scroll; text absolutely positioned over edge-to-edge art.

## Pages

| Route | What it is |
|-------|-----------|
| `/` | Hero + marquee, count-up stats strip, four full-bleed rendered "regions", manifesto, mint CTA |
| `/gallery` | Filterable monochrome collection grid (grayscale → color on hover), lineage chips, live count |
| `/lore` | Cinematic story chapters + the four-lineage breakdown + pull quote |
| `/shop` | Functional mint panel — tier/quantity selector, live price total, mint progress meter, FAQ |

## Interactions & effects

Scroll-reveal (IntersectionObserver), scroll-triggered underline marks, parallax on art layers, count-up numbers, animated marquee, slow hero zoom, scan-line preview, nav solidify-on-scroll, mobile drawer, wallet-connect modal, toast notifications, gallery filtering, and a live-calculating mint interface.

> Content (imagery + copy) is placeholder — cinematic stock photos standing in for 3D game renders, plus generated lore/marketing copy. Wallet/mint flows are simulated (nothing is signed or charged).

## Run

```bash
npm install
npm run dev      # http://localhost:4321
npm run build    # static output in dist/
```
