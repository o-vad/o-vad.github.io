# O-VAD — Project Page

Project page for **O-VAD: Industrial Video Anomaly Detection through Object-Centric Tracking and Reasoning** (ECCV 2026).

## Deploy to GitHub Pages

1. Create a repo (e.g. `o-vad.github.io`) and push every file in this folder.
2. In **Settings → Pages**, set the source to the `main` branch, root (`/`).
3. The page goes live at `https://<user>.github.io/<repo>/`.

`index.html` is self-contained — it loads its runtime and React from a CDN at page load, so no build step is required.

## Files

```
index.html            ← the page GitHub Pages serves (entry point)
O-VAD.dc.html         ← editable source (same content as index.html)
support.js            ← page runtime (required, keep next to index.html)
figures/
  intro.pdf           ← source figures (as cited by the paper)
  framework.pdf
  2cases.pdf
  servo-magnet.pdf
  buttion-clip.pdf
  liquid-stickyroller.pdf
  intro.png           ← raster shown on the page (Fig. 1 / teaser)
  framework.png       ← raster shown on the page (Fig. 2 / pipeline)
  liquidad_masks.png  ← LiquidAD instance masks
  liquidad_f1..3.jpg  ← LiquidAD tracked-pipette frames
static/
  videos/
    demo.mp4          ← demo video
```

## Figures

The page displays `figures/intro.png` and `figures/framework.png`. The matching source PDFs are in the same directory. To regenerate the PNGs at higher DPI, export the PDFs with any of:

```bash
# poppler
pdftoppm -png -r 300 figures/framework.pdf figures/framework
# or ImageMagick
magick -density 300 figures/framework.pdf figures/framework.png
# or macOS
sips -s format png figures/framework.pdf --out figures/framework.png
```

Keep the output filenames (`intro.png`, `framework.png`) and the page picks them up with no HTML edits.

## Edit the content

Open `index.html` and edit text directly. The Code button and BibTeX default to `github.com/o-vad/O-VAD` — update to your real repo. The accent color is set via `--accent` near the top of the file (also exposed as a tweak).
