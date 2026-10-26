# hytiger.github.io

GitHub Pages user site, used as the shared **developer website** for all hytiger apps on Google Play.

- `app-ads.txt` — AdMob authorized sellers file, shared by every app. Must stay at the site root:
  https://hytiger.github.io/app-ads.txt
  One line per ad account (not per app). Add lines only for a new AdMob account or mediation network.
- `index.html` — hub page listing each app (Play link, privacy policy).
- `.nojekyll` — serve files as-is.

Privacy policies live in a separate repo per app, served as project pages
(e.g. `barofx-privacy` → https://hytiger.github.io/barofx-privacy/).

## Adding a new app

1. Create a `<app>-privacy` repo and enable GitHub Pages on it.
2. Copy a `<section class="app">` block in `index.html` and fill in the name, description, Play link and privacy link.
3. In Play Console (Store settings → contact details), set the website to **https://hytiger.github.io**.
4. In AdMob, open the app-ads.txt page and use "Check for updates".
