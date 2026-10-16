# ZedOffline

A tiny offline-first sales and expense tracker for Android Chrome.

## Features
- Record sales and expenses in Zambian kwacha
- Today's sales, expenses and net total
- Local browser storage (no account/server)
- Export/import JSON backup
- PWA service worker cache for offline reopening

## Publish from an Android phone with GitHub Pages
1. Extract this ZIP using your phone's file manager.
2. In Chrome, sign in or create an account at https://github.com.
3. Create a new public repository named `zedoffline` (or another name).
4. Use **Add file → Upload files** and upload `index.html`, `manifest.json`, and `sw.js` from this folder to the repository root. Commit the files.
5. Open repository **Settings → Pages**. Under Build and deployment, choose **Deploy from a branch**, select `main` and `/ (root)`, then Save.
6. Wait for GitHub Pages to publish. Open the Pages URL shown in Settings → Pages, e.g. `https://YOUR-USERNAME.github.io/zedoffline/`.
7. While online, open the page in Chrome and wait for it to load fully. Open it again once while still online.
8. In Chrome's three-dot menu choose **Install app** or **Add to Home screen**, if offered.
9. Test: open the installed app, turn on Airplane mode, close and reopen it. Add a test sale, close/reopen, and confirm the record remains.

## Important
- The app's interface and saved records work offline after caching on the published HTTPS site.
- Records are saved only in this browser/app profile on this phone. They do not sync to other devices.
- Export a backup regularly. Clearing Chrome/site data, uninstalling, or resetting the phone can delete records.
- Never use it as your only record for important finances. Check totals and keep another backup.
- Do not put real customer secrets or passwords in this app.
- If you update app files later, increment `CACHE_NAME` in `sw.js` (e.g. `zedoffline-v2`) to refresh the offline cache.
