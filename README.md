# حاسبة الطلبية — installable offline app (PWA)

Upload the **contents of this folder** to any HTTPS host. Phones only install apps and enable offline mode over HTTPS.

## Option A — GitHub Pages (free, permanent)
1. Create a free account at github.com, then **New repository** (e.g. `talabiya`, Public).
2. **Add file → Upload files** and drag in everything from this folder: `index.html`, `sw.js`, `manifest.webmanifest`, and the `icons` folder. Commit.
3. **Settings → Pages → Build and deployment**: Source = *Deploy from a branch*, Branch = `main`, folder `/ (root)`. Save.
4. After about a minute the app is live at `https://YOUR-NAME.github.io/talabiya/`.

## Option B — Netlify Drop
Log in to a free Netlify account, open app.netlify.com/drop and drag this whole folder onto the page.

## Install on your phone
- **Android (Chrome):** open the link → Settings tab → **تثبيت التطبيق**, or Chrome menu ⋮ → *Install app*.
- **iPhone (Safari):** open the link → Share button → *Add to Home Screen*.

Open it once while online so it saves the Excel tool and the Arabic font. After that it works with no internet.

## Updating later
Change the files, and bump `VERSION` in `sw.js` (e.g. `talabiya-v1.1.1`) so phones fetch the new version. The update shows the next time the app is opened.

## Your data
Data is stored on the phone, inside the app. On iPhone the installed app keeps its own storage, separate from Safari, so enter your data in the installed app (or move it over with Settings → Export / Import backup).
