# O-VAD — Project Page

Project page for **O-VAD: Industrial Video Anomaly Detection through Object-Centric Tracking and Reasoning** (ECCV 2026).

## Deploy to GitHub Pages

1. Create a repo (e.g. `o-vad.github.io`) and push every file in this folder.
2. In **Settings → Pages**, set the source to the `main` branch, root (`/`).
3. Your page goes live at `https://<user>.github.io/<repo>/`.

`index.html` is self-contained — it loads its runtime and React from a CDN at page load, so no build step is required.

## Files

```
index.html            ← the page GitHub Pages serves (entry point)
O-VAD.dc.html         ← editable source (same content as index.html)
support.js            ← page runtime (required, keep next to index.html)
static/
  images/
    teaser.png        ← Figure 1 (intro)          — rendered from the paper
    pipeline.png      ← Figure 2 (framework)       — rendered from the paper
    liquidad_masks.png← LiquidAD instance masks
    liquidad_f1..3.jpg← LiquidAD tracked-pipette frames
  videos/
    demo.mp4          ← (add your demo video here)
```

## Before publishing

- **Demo video** — drop your walkthrough at `static/videos/demo.mp4` (the teaser image shows as the poster until then).
- **Code link** — the Code button and BibTeX default to `github.com/o-vad/O-VAD`; update to your real repo (search that string in `index.html`, or edit the `githubUrl` tweak).
- **Figures** — `teaser.png` and `pipeline.png` are rasterized from `intro.pdf` / `framework.pdf` at ~910px. If you want crisper versions, export those PDFs to PNG yourself and overwrite the files (same names).

## Edit the content

Open `index.html` and edit text directly. The accent color is set via `--accent` near the top of the file (also exposed as a tweak).
