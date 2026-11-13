# 12bajay workout

A personal workout, nutrition and progress tracker. All data stays in the browser on the device that uses it.

## Files
- `index.html`: the whole app (HTML, CSS and JavaScript in one file)
- `manifest.json`, `service-worker.js`: install to home screen and work offline
- `icons/`: app icons and logo
- `favicon.ico`: browser tab icon
- `404.html`: page shown for unknown links
- `netlify.toml`: Netlify publish settings

## Deploy
Upload this folder to Netlify (or any static host with HTTPS). Home-screen install and offline use need HTTPS.

## Custom domain
Netlify: Site settings > Domain management > Add a domain. Point your domain's DNS at Netlify as shown there.

## Backup
Use Menu > Export backup regularly. On iPhone, the home-screen app stores its data separately from Safari, so import the backup into the app you use.
