# ShoalWatch

Early warning and collective biosecurity for farms that share water. An installable web app (PWA) that works offline.

## Put it on GitHub Pages

1. Create a new public repository on GitHub (for example `shoalwatch`).
2. Upload everything in this folder to the **root** of the repository, keeping the `icons` folder:
   `index.html`, `manifest.webmanifest`, `sw.js`, `config.js`, `.nojekyll`, `icons/`
3. In the repository go to **Settings → Pages**. Under **Build and deployment** choose **Deploy from a branch**, pick `main` and `/ (root)`, then **Save**.
4. After a minute your app is live at `https://YOUR-USERNAME.github.io/shoalwatch/`.

## Install on Android (Chrome)

Open the link in Chrome. Tap the **Install app** button inside ShoalWatch, or Chrome's own install banner. If neither shows, use the Chrome menu (three dots) → **Install app**. On iPhone, use Safari → Share → **Add to Home Screen**.

## Updating the app

After you change any file, edit `VERSION` in `sw.js` (for example `shoalwatch-v2`) so phones fetch the new files.

## Optional shared database

Data stays on each device by default. To sync through Supabase, fill in `config.js` with your project URL and the public **anon** key only. Never put a service key in this file, because GitHub Pages makes it public.

## Notes

- Old Nerissa records on a phone are copied across automatically the first time ShoalWatch opens on the same address.
- Before collecting real farmer data, agree your consent wording and check your university's IP policy and TAGDev 2.0 terms.
