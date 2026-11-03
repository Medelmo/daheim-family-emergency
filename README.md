# Daheim – Familien-Notfallplan (PWA)

A free, dependency-free, German/Arabic offline-first family preparedness app.

## Features
- Installable PWA with manifest, app icons and service worker
- Offline app shell after the first successful load
- IndexedDB storage for supplies and checklist state
- Automatic migration from the previous `daheim-items` / `daheim-checks` localStorage keys when run on the same origin
- Supply inventory with quantity, category, storage location and expiry status
- 10-step household checklist
- Drinking-water estimate calculator
- JSON export/import backup
- Responsive desktop/mobile layout and RTL Arabic interface

## Run locally
Serve this folder over `http://localhost` (not by opening `index.html` as a file):

```bash
python -m http.server 8080
```

Then open http://localhost:8080. Service workers and installability require HTTPS in production, or localhost for development.

## Free hosting
Deploy the folder as a static site on a free HTTPS static host (for example GitHub Pages or Cloudflare Pages). No backend or account is needed by the app itself. The source files can be hosted publicly, but the family's inventory and checklist data stay in the browser's IndexedDB and are not uploaded.

## Data and privacy
- No analytics, advertising, external fonts, remote APIs or third-party JavaScript.
- Data is stored locally in the browser profile on the device.
- The JSON backup contains the household's entries; store it privately.
- Clearing browser/site data or uninstalling/clearing the browser profile can remove local data. Export backups regularly.
- No automatic sync between devices.

## Sources and licenses
- No external UI framework or component library is bundled. UI is custom CSS/HTML using native platform controls and system fonts.
- PWA platform behavior follows the web standards documented by MDN: https://developer.mozilla.org/en-US/docs/Web/Progressive_web_apps/Guides/Making_PWAs_installable
- App code and original icon artwork in this package are provided for reuse under the MIT License (see LICENSE).
