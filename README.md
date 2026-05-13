# Raw Flash — Public web assets

Static pages served alongside the app, required by App Store Connect / Apple Review.

## Files

| File | Purpose |
|---|---|
| `privacy.html` | Privacy policy (Italian + English) — bound to the **Privacy Policy URL** field in App Store Connect |

## Publishing via GitHub Pages (recommended, free)

1. Create a public repo (e.g. `rawflash-web`) and push the contents of this folder to its `main` branch
2. In the repo settings → **Pages** → set **Source = `main` branch / root** → save
3. After ~1 minute, the URL `https://<username>.github.io/rawflash-web/privacy.html` becomes live
4. Paste that URL into App Store Connect → App Information → **Privacy Policy URL**

Alternatively, if you prefer a custom domain (e.g. `rawflash.app/privacy`), point a `CNAME` to GitHub Pages and serve from there.

## Updating

Re-publishing is just a `git push` — GitHub Pages re-deploys in seconds.

Bump the date at the top of `privacy.html` (both English and Italian) whenever the substance changes. The date is the only source of truth for "when did this last get edited?" — Apple Review checks it.
