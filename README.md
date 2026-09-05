# MyMood — product site

The official site for **MyMood**, a private mood journal for iPhone.
Live at <https://lauromarinho.github.io/mymood-landing/>.

Static HTML and one stylesheet, served by GitHub Pages from `main` at the repo root.
No build step, no dependencies — edit a file, push, done.

## Pages

| File | URL | Notes |
| --- | --- | --- |
| `index.html` | `/mymood-landing/` | The product home page |
| `privacy.html` | `/mymood-landing/privacy.html` | **Do not rename.** This exact URL is hardcoded in the app (`SettingsView.swift`, `ProPaywallView.swift`) and registered in App Store Connect |
| `terms.html` | `/mymood-landing/terms.html` | Terms of Use and subscription terms |
| `support.html` | `/mymood-landing/support.html` | Support and how-to, good as the App Store support URL |
| `styles.css` | — | Shared design system for all four pages |

## Assets

- `assets/app-icon.png` — the 1024pt app icon, copied from
  `MyMood/Assets.xcassets/AppIcon.appiconset/1024.png`. Re-copy it if the icon changes.
- `assets/screens/` — screenshots. See the [README there](assets/screens/README.md) for the
  exact filenames; the page shows a dashed placeholder until each file exists.
- `assets/og.jpg` — 1200×630 link-preview image. Referenced by the Open Graph tags but not
  committed yet, so shared links currently show no image.

## Before publishing changes

- **Prices.** The Pro card in `index.html` shows €9.99/year and €1.99/month. Confirm those
  against App Store Connect; they're marked with an HTML comment.
- **Dates.** `privacy.html` and `terms.html` each carry a "Last updated" date. Bump it when
  the text changes materially.
- **Free/Pro limits.** The comparison table mirrors `Services/ProLimits.swift` in the app.
  If the limits move there, move them here too.

## Design

Warm paper, purple ink, serif headlines — the site is meant to feel like the object the app
imitates. The accent purple is the same one the app uses (`Palette.accent`). Light and dark
are both defined explicitly via `prefers-color-scheme`.
