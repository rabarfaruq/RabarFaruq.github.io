# Reel Board — install as an app

This folder is a complete, installable web app. Put it on GitHub Pages and
you can add it to your home screen on both Android and iPhone, and it keeps
working even with no internet connection once it's been opened one time.

## Files in this folder

- `index.html` — the app itself
- `manifest.webmanifest` — tells Android/iOS how to install it (name, icon, colors)
- `sw.js` — service worker, caches the app so it loads offline
- `icon-*.png`, `favicon.png` — the app icons

Keep all of these files together, in the same folder, when you upload them.

## Option A — new repo just for this

1. On GitHub, create a new repository, e.g. `reel-board`.
2. Upload every file in this folder to the root of that repo (drag-and-drop
   on the GitHub website works fine — "Add file" → "Upload files").
3. Go to the repo's **Settings → Pages**.
4. Under **Source**, choose **Deploy from a branch**, branch `main`, folder `/ (root)`. Save.
5. After a minute, your app is live at:
   `https://<your-username>.github.io/reel-board/`

## Option B — a folder inside your existing rabarfaruq.github.io site

Since you already have `rabarfaruq.github.io`, you can add this as a
sub-page instead of a separate repo:

1. In that repo, create a folder called `reel-board`.
2. Upload every file from this folder into `rabarfaruq.github.io/reel-board/`.
3. It'll be live at:
   `https://rabarfaruq.github.io/reel-board/`

No separate Pages setup needed — your existing site's Pages config already
covers it.

## Installing it on your phone

Once the link above works in a mobile browser:

**iPhone (Safari):**
Open the link → tap the Share button → **Add to Home Screen** → Add.

**Android (Chrome):**
Open the link → Chrome will usually show an **Install app** banner or
you can tap the ⋮ menu → **Install app** / **Add to Home screen**.

Either way you get a real app icon on your home screen that opens full-screen,
no browser bars — and it'll keep working even in airplane mode after that
first open.

## A note on your data

Your reels save to that browser's local storage on that specific device.
Opening the same GitHub Pages link on a different phone or computer starts
fresh there — it isn't synced between devices. If you want that later,
that would mean adding a real backend, which is a bigger step.
