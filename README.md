# LINE SHIFT — iPhone-ready web app

This is a ready-to-publish, static Progressive Web App. No framework, build tools, backend, or paid hosting are needed.

## What it includes

- 3–4 local/pass-and-play players, computer opponents, or a mix
- Default **five in a row on 9×9**; four in a row is available as an optional classic rule
- One action per turn: place one stone **or** push a continuous line of stones one cell
- Reverse-push protection that follows the moved stones until the pushing player completes the next turn
- Undo, restart, move history, and automatic save/restore on the same device
- Installable iPhone Home Screen icon and offline play after initial successful online load

## Publish free with GitHub Pages

1. Sign in to [GitHub](https://github.com/) and create a new **public** repository, e.g. `line-shift`.
2. Choose **Add file → Upload files**. Upload the **contents of this folder**, including `index.html`, `sw.js`, `manifest.webmanifest`, `.nojekyll`, and the three `.png` icons. Do not upload the ZIP itself as the site. Commit the files.
3. Open the repository's **Settings → Pages**. Under **Build and deployment**, choose **Deploy from a branch**, select **main** and **/(root)**, then click **Save**.
4. GitHub will display a site URL like `https://YOUR-USERNAME.github.io/line-shift/`. Open that address.

## Add to your iPhone Home Screen

1. Open your hosted URL in **Safari** on iPhone.
2. Tap **Share** (on some Safari layouts, tap the page menu then Share).
3. Tap **Add to Home Screen**, leave **Open as Web App** enabled, then tap **Add**.
4. Launch LINE SHIFT from its Home Screen icon.

Once loaded successfully online, the Home Screen app works offline. A saved game is kept in your browser/app's device storage, not synced to other devices.

## Test locally

`index.html` can be opened as a local HTML file for a quick preview, but a service worker/offline installation requires an HTTPS host (or `localhost` during development). To test locally with Python, run `python3 -m http.server 8000` from this folder, then open `http://localhost:8000`.

## Limits

This is a **web app**, not a native iOS App Store build. Publishing in the Apple App Store requires a separate iOS wrapper or native app, Apple developer setup, and app review. There is no online multiplayer; all human players share one device.
