# RBC Reading Empire

A self-contained reading tracker for *The Worldly Philosophers* by Robert L. Heilbroner.
It runs entirely in the browser. No build step, no server, no dependencies.

## What you actually need to upload

Just one file: `index.html`.

The RBC logo is baked into the HTML as a base64 image, and every sound (the timer
chime, the milestone ding, the victory fanfare) is generated in the browser with the
Web Audio API. So there are no separate picture or audio files to upload.

The `assets/RBC_Royal_Bank.png` in this folder is the original logo, kept here only in
case you want it on hand. The game does not load it, so you can ignore or delete it.

## Deploy to GitHub Pages

1. Create a new public repository on GitHub.
2. Upload `index.html` to the root of the repo. Keep the name `index.html` so Pages
   serves it as the home page.
3. In the repo, go to Settings, then Pages.
4. Under "Build and deployment", set Source to "Deploy from a branch".
5. Choose your branch (usually `main`) and the `/ (root)` folder, then Save.
6. Wait about a minute, then open `https://YOUR-USERNAME.github.io/YOUR-REPO/`.

Your reading progress is saved in the browser (localStorage) on whichever device you
open it on. It does not sync across devices.

## Running it locally

Double-click `index.html` to open it in any browser. Everything works offline,
including the timer and all sounds.
