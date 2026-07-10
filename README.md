# STLARviz

AR viewer for **STL** 3D models, built with [A-Frame](https://aframe.io/) and [AR.js](https://ar-js-org.github.io/AR.js-Docs/). Point your phone camera at a **Hiro** marker and your model appears in augmented reality.

![STLARviz](https://img.shields.io/badge/A-Frame-1.6.0-blue) ![AR.js](https://img.shields.io/badge/AR.js-3.4.7-orange)

## Features

- **STL loading** — from a local file (`Browse`), a pasted URL (`Load`), or by **scanning a QR code** (`Scan QR`) that links to an `.stl` file.
- **Binary & ASCII STL** — both formats parsed in-browser.
- **Transform controls** — rotate (X/Y/Z), scale, and distance sliders.
- **Touch rotation** — drag the camera view to spin the model.
- **Color swatches** — switch the model material color.
- **Auto-fit** — geometry is centered and auto-scaled to the marker.
- **Transparent camera feed** — the model overlays the live video.

## Usage

1. Open the app (deployed URL or local server).
2. Tap **Browse** to pick a `.stl` file, paste an STL URL and tap **Load**, or tap **Scan QR** and point the camera at a QR code whose link ends in `.stl`.
3. Point your device camera at a [Hiro marker](https://raw.githubusercontent.com/AR-js-org/AR.js/master/data/images/hiro.png).
4. Drag the camera view to rotate; use the sliders and swatches to adjust.

> Tip: On desktop without a camera, the scene still loads — you just won't see AR tracking.

## Tech

- `index.html` — single-file app (markup, styles, parser, and UI logic).
- `vercel.json` — serves the repo as a static site on Vercel.

## Deploy

This repo is configured for [Vercel](https://vercel.com/) static hosting.

```bash
# install CLI and link
npm i -g vercel
vercel
```

Or import the GitHub repo directly in the Vercel dashboard — no build step required.

## License

Add a license as needed.
