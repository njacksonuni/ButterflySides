# Butterfly Sides — Slidedeck Plan

## 1. Image assessment
The repo contains three JPGs (the `pictures/bin` file is an empty placeholder):

| File | Subject | Scene | Notes |
|------|---------|-------|-------|
| `Schmetterling1jpg.jpg` | Monarch (*Danaus plexippus*) | Wings open on a yellow flower in grass | Orange panels, black veins, white-dotted border |
| `Schmetterling2.jpg` | Blue Morpho (*Morpho peleides*) | Wings open flat on grey stone | Iridescent structural-blue, black dotted edge |
| `Schmetterling3.jpg` | Black Swallowtail (*Papilio polyxenes*) | Wings folded on pink ironweed | Yellow/blue spots, orange eyespot |

All are small (~8–17 KB), web-ready, landscape-ish. No optimization needed.

## 2. Goals
- **Responsive** single-page slidedeck (works phone → desktop).
- **Accessible** — descriptive `alt` text on every image.
- **Fun, detailed** species descriptions + a "fun fact" per slide.
- **Quilt-inspired aesthetic** throughout.

## 3. Approach
- Self-contained `index.html` (no build step, no dependencies) so it opens
  anywhere and survives the ephemeral container.
- **Layout:** CSS Grid `auto-fit` patchwork — slides reflow into 1/2/3
  columns as the viewport grows; each slide is a stitched "patch."
- **Quilt styling:**
  - Calico checker background using layered diagonal gradients.
  - Each patch double-bordered (cream + dark "thread") with dashed
    "stitching" dividers and a corner badge button.
  - Rotating 4-colour patch palette (terracotta / teal / goldenrod / heather).
  - Diagonal-stripe "fabric" matte inside each photo frame.
- **A11y:** semantic `<article>`/headings, keyboard-focusable slides,
  `prefers-reduced-motion` support, high-contrast text.

## 4. Possible future patches
- Add more butterfly images as new `<article>` slides (palette auto-rotates).
- Optional lightbox / keyboard arrow navigation for a true "deck" mode.
- Replace placeholder `pictures/bin` with real assets.
