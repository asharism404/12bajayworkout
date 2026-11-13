# 12bajay workout — installable PWA

This is the original single-file web app with Progressive Web App support added. Existing workout logic and local browser storage were left intact.

## Deploy

Upload the complete folder to your existing static host (Netlify, Vercel, or GitHub Pages). Keep `index.html`, `manifest.json`, `service-worker.js`, and the `icons/` directory together at the same site path. HTTPS is required for service workers; these hosts provide it.

## Install on Android

1. Open the deployed site in Chrome.
2. Use **Install app** from the browser menu or the install prompt if Chrome offers one.
3. Confirm the installation.

## Install on iPhone

1. Open the deployed site in **Safari** (not an in-app browser).
2. Tap **Share** → **Add to Home Screen**.
3. If shown, enable **Open as Web App**, then tap **Add**.

## Offline and data notes

- The app shell and same-origin files are cached for offline launching after the first successful online visit.
- Workout data continues to use the browser's existing local storage. Installing the PWA does not automatically transfer data between browsers or devices.
- External Google Fonts and other network-dependent services may not load offline.
- This is not a full offline sync system. Test important flows after deployment.
- To force clients to refresh the service worker after a future release, change `CACHE_NAME` in `service-worker.js` (for example, `v1` to `v2`).

## Files added

- `manifest.json` — app name, theme, display mode and icon declarations.
- `service-worker.js` — app-shell caching and offline navigation fallback.
- `icons/` — Android and iOS home-screen icons.

## Custom domain
Netlify: Site settings > Domain management > Add a domain. Buy the domain from any registrar and point it at Netlify. `404.html` is served automatically for unknown URLs.
