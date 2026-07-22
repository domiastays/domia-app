# Domia Guest Guide — deploy to GitHub Pages

This folder IS the website. Everything is here. No build step, no terminal.

## Files
- `index.html` ............ the guest app (edit the CONFIG block for each apartment)
- `manifest.webmanifest` .. makes it installable as an app
- `sw.js` ................. offline support (network-first, so edits show instantly)
- `domia-icon.png` ....... app / home-screen icon
- `domia-logo.png` ....... footer logo (official gold-on-navy)
- `photo.jpg` ............ the property photo shown in the header

## Put it live (all in the browser — no commands)
1. Go to github.com → **New repository**. Name it `guest-guide`. Public. Create.
2. On the empty repo page click **"uploading an existing file"**.
3. Drag in ALL the files from this folder (index.html, manifest.webmanifest, sw.js,
   the 3 images). Click **Commit changes**.
4. Repo → **Settings → Pages**. Under "Build and deployment" set
   **Source: Deploy from a branch**, **Branch: main / (root)**. Save.
5. Wait ~1 minute. Your live link is:
   **https://domiastays.github.io/guest-guide/**

(Optional, later) point a custom subdomain like `guide.domiastays.es` to it in
Settings → Pages → Custom domain.

## Where you edit / add info later
- On github.com, open the repo → click **index.html** → the **pencil (Edit)** icon.
- Change only the **CONFIG block at the top** (name, address, code, WiFi, WhatsApp,
  recommendations). Scroll down, **Commit changes**. The live site updates in ~1 min.
- To change the photo: upload a new `photo.jpg` (same name) — Add file → Upload.

## New apartment = new guide
Make another repo (e.g. `guide-sunset`), upload the same files, edit its CONFIG and
photo. Each apartment gets its own link + its own QR.
