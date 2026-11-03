# Deployment and installation

Daheim is a static Progressive Web App. It requires HTTPS in production (GitHub Pages provides HTTPS).

## GitHub Pages
1. Open repository Settings → Pages.
2. Under Build and deployment, select Deploy from a branch.
3. Select `main` and `/(root)`, then Save.
4. Wait for the deployment to finish. The site URL will be `https://medelmo.github.io/daheim-family-emergency/`.
5. Open that URL in Chrome on Android and choose Install app or Add to Home screen.

## Privacy
The source code is public. The household inventory and checklist are stored locally in the browser using IndexedDB. Do not commit JSON backup files. Export backups and keep them somewhere private.

## Moving to a NAS
Copy the complete static site to a web server on the NAS and serve it over HTTPS. Keep the same origin if you want the browser's existing IndexedDB data to remain available; changing domains/origins does not automatically move local data. Export a JSON backup before migrating and import it on the new origin.
