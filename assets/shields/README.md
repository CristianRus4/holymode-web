# Shield artwork

`Shield02.png` … `Shield30.png` — the collectible shields, at 900 × 990 RGBA.

These are **app assets, not site content**. Nothing on the site links to them.
They live here so the app can ship without ~31 MB of artwork nobody has earned
yet: HolyMode bundles `Shield01` only and downloads the rest on demand once a
subscription is active, caching them on the device.

Served from `https://cristianrus4.github.io/holymode-web/assets/shields/`.
The app's base URL is `AppConstants.shieldArtworkBaseURL`; change both together.

Do not rename these. The filenames are the app's slot numbers, and the slot order
is a product decision recorded in the app repo's revision brief — the artwork a
given number points at can change between revisions.
