# holymode-web

The marketing site for **HolyMode**, an iPhone app that helps Christian men quit porn — it blocks tempting apps and sites with Apple Screen Time, gives a daily Bible verse, tracks a streak of days you stood firm, unlocks 30 collectible shields, and offers an optional community. Recovery data stays on the device.

Live at **https://cristianrus4.github.io/holymode-web/**.

## What's here

| File | Purpose |
| --- | --- |
| `index.html` | Landing page: hero, download link, feature blocks, footer |
| `privacy.html` | Privacy policy |
| `terms.html` | Terms of service |
| `styles.css` | All styling — dark theme, gold accent, mobile-first |
| `CNAME` | Custom domain for GitHub Pages |

Plain static HTML and CSS. No build step, no framework, no external requests — open `index.html` in a browser, or run `python3 -m http.server` in this directory to preview.

## Before launch

The App Store button in `index.html` is a placeholder (`href="#"`). Search for the `TODO` comment above it and swap in the real App Store URL, then remove the "Coming soon." note under the button.

## Deploying to GitHub Pages

Pages serves the default branch root, so any push to `main` publishes.

```sh
git add -A
git commit -m "Update site"
git push
```

### One-time setup

1. **Enable Pages.** Repo → Settings → Pages → *Build and deployment* → Source: **Deploy from a branch**, Branch: **main**, Folder: **/ (root)**.
2. That is all. The site serves from `https://cristianrus4.github.io/holymode-web/`.

### Custom domain

The `CNAME` file at the repo root holds the custom domain and is what GitHub
Pages reads to know which host to serve. Deleting it unsets the custom domain
and the site goes back to the `github.io` address, so leave it alone unless the
site is being moved off Pages.

DNS for the domain lives with the registrar, not here: four apex `A` records to
`185.199.108.153`, `.109.153`, `.110.153`, `.111.153`, all unproxied. Proxying
blocks the HTTP validation Pages uses to issue its certificate.

All links in the pages are relative, so the site works on either host.
