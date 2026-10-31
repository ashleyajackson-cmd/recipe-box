# Recipe Box — Simple Setup

No database, no sign-up, no SQL. One step.

## 1. Host it (Netlify, free)

1. Go to https://netlify.com and sign up.
2. From the dashboard, find "Add new site" → "Deploy manually" (or the drag-and-drop box on the main page).
3. Drag the whole `simple-app` folder onto the upload area — or drag all five files inside it: `index.html`, `manifest.json`, `sw.js`, `icon-192.png`, `icon-512.png`.
4. Netlify gives you a URL like `https://random-name-123.netlify.app`. That's it — the app is live.

## 2. Add it to your home screen (iPhone)

1. Open the Netlify URL in **Safari** (must be Safari, not Chrome).
2. Tap the **Share** button (square with an arrow) at the bottom.
3. Tap **"Add to Home Screen"**, then **Add**.

You now have a Recipe Box icon that opens full-screen, like a normal app. All 84 recipes are already loaded in — nothing else to do.

## How this version works

- Everything saves directly in Safari's own storage on your phone — no external service, no login, nothing to configure.
- Data is specific to this one device. If you want the same recipes on another phone or a computer, open the same Netlify URL there — it'll load the 84 built-in recipes fresh, but anything you've personally added or edited on your phone won't carry over automatically.
- Backup tip: if you want a safety copy of your recipes, use the "Copy" button on any recipe (or the whole shopping list) to paste it somewhere like Notes as a backup — there's no automatic export yet, but I can add one if useful.
- If you ever clear Safari's website data/history for this site, the recipes stored there would be cleared too — this is rare but worth knowing.

If you outgrow this later and want real multi-device syncing, that's what the Supabase version was for — we can revisit it once this simpler version is solid.
