# Kala 3 — Bol Property Website

A static, multilingual (EN / SL / HR / IT / FR) one-property website for the stone
house at Kala 3, Bol, island of Brač, Croatia.

## Contents
- `index.html` — the whole site (home, surroundings, opportunity, contact)
- `support.js` — runtime the page needs (keep it next to index.html)
- `images/` — all photos, floor plans, the map, and `view.mp4`

## Deploy (GitHub → Netlify)
1. Create a new GitHub repository and push these files to it (see steps below).
2. In Netlify: **Add new site → Import an existing project → GitHub**, pick the repo.
3. Leave **Build command** empty and set **Publish directory** to `.` (root).
   The included `netlify.toml` already sets this.
4. Deploy. Netlify gives you a live URL; add a custom domain later if you like.

## Images
Photos are pre-optimised for the web: resized to a max of 2000px (2560px for the
hero) and re-encoded with mozjpeg. Several photos that were shipped as PNG are now
JPEG, so the filenames in the `interior` / `exterior` lists in `index.html` differ
from the originals. Note that `bedroom-3.png` became `bedroom-3-alt.jpg`, because
`bedroom-3.jpg` is a different photo.

Full-resolution originals are in git history at commit `5dd599b`. Re-exporting this
site from Claude Design will overwrite the optimised files with the originals again.

## Editing later
- Contact phone/email are placeholders in `index.html` — search for
  `+385 00 000 0000` and `info@kala3.example` and replace with real details.
- All text lives in the language tables inside `index.html`.
