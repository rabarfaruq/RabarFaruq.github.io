# Reel Board — already wired into rabarfaruq.github.io

This folder sits inside your `RabarFaruq.github.io` repo. Your site's
navbar already links to it (the "Reel Board" item added to `index.html`
one level up). Once you push both, it'll be live at:

`https://rabarfaruq.github.io/reel-board/`

## Files in this folder

- `index.html` — the app itself
- `manifest.webmanifest` — tells Android/iOS how to install it
- `sw.js` — service worker, caches the app so it works offline
- `icon-*.png`, `favicon.png` — app icons

## What changed in your repo

One line was added to the `<ul class="nav-links">` in your root
`index.html`:

```html
<li><a href="reel-board/index.html" target="_blank" rel="noopener">Reel Board</a></li>
```

It opens in a new tab so people browsing your portfolio don't lose their
place. Everything else in your site is untouched.

## Installing it on your phone

Once `rabarfaruq.github.io/reel-board/` is live:

**iPhone (Safari):** open the link → Share → **Add to Home Screen**
**Android (Chrome):** open the link → **Install app** (banner or ⋮ menu)

You get a real home-screen icon, opens full-screen, and works offline
after the first visit.

## Uploading this to GitHub

1. In your `RabarFaruq.github.io` repo, replace the existing `index.html`
   at the root with the one included alongside this folder.
2. Upload this whole `reel-board` folder into the repo root (so the final
   path is `RabarFaruq.github.io/reel-board/index.html`, etc.).
3. Push / commit. GitHub Pages will pick it up automatically — no Pages
   settings changes needed since your repo is already configured.
