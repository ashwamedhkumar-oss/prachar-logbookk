# prachar-logbookk

Standalone logbook for Prachar DOOH.

## What this is
- Single static `index.html` that runs in the browser.
- Attempts to auto-import locations from https://prachardooh.com/where-we-are (best-effort).
- Stores bookings in localStorage (no backend).
- Meant to be hosted on GitHub Pages (or any static host) and embedded in Hostinger AI via an iframe.

## How to use
1. Upload `index.html` to the root of a public GitHub repository (see instructions).
2. Enable GitHub Pages (branch `main`, folder `/ (root)`).
3. Embed with iframe in Hostinger AI:
   `<iframe src="https://YOUR_GITHUB_USER.github.io/prachardooh-logbook/" style="width:100%;height:720px;border:0;"></iframe>`

## Notes
- Auto-import uses public CORS proxies; if proxies fail, paste locations manually into the right-hand textarea.
- For multi-user live sync, a small server (PHP/Node) is needed — I can generate that later.
