# tastedex.github.io

Static landing page for TasteDex recipe share links.

When a user taps a shared recipe URL like
`https://tastedex.github.io/?d=<gzipped-base64-json>`, Android routes the
tap directly to the TasteDex app if it's installed (verified via
`/.well-known/assetlinks.json`). If the app isn't installed, the user
sees a simple "Open in TasteDex / Get it on Google Play" card.

No server, no tracking — just two static files:
- `index.html` — the landing page + deep-link redirect
- `.well-known/assetlinks.json` — Android App Links verification
