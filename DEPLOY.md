# Publish the app for installation

A PWA cannot be installed from a downloaded `file://` HTML file. It must be served from HTTPS (or localhost during development).

## GitHub Pages (free)
1. Create a new GitHub repository. Choose public only if you are comfortable publishing the app's source code; the app does not contain your family data.
2. Upload the *contents* of this folder to the repository root.
3. In **Settings → Pages**, choose **Deploy from a branch**, select `main` and `/ (root)`, then save.
4. Wait for the Pages deployment and open the HTTPS URL on your Android phone.
5. In Chrome, use **Install app** / **Add to Home screen**. On supported browsers the app opens in its own window.

If you prefer not to publish the source publicly, use a private repository with a hosting service/plan that supports private deployments, or a static hosting provider with a free private-project option. Do not upload a backup JSON file to the repository.
