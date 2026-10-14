# Shaadi Planner site

Support page and privacy policy for the Shaadi Planner TestFlight beta, served with GitHub Pages.

| Page | File |
|---|---|
| Support (Marketing URL) | `index.html` |
| Privacy policy | `privacy.html` |

Plain static HTML and one stylesheet, no build step. Colours and fonts match the app (Rea's dark plum and gold, Playfair Display titles).

## Before publishing

Swap the placeholder email everywhere:

```sh
sed -i '' 's/you@example.com/YOUR_REAL_EMAIL/g' index.html privacy.html
```

## Turn on GitHub Pages

Settings → Pages → Build and deployment → Deploy from a branch → `main` / `(root)` → Save.

The site goes live at `https://<github-username>.github.io/<repo-name>/` and the privacy policy at `.../privacy.html`. A custom domain can be added later from the same screen.

## When to update

Update `privacy.html` (and its effective date) before any build that adds sync, family sharing, analytics, purchases or anything else that sends data off the device.
