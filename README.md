# lorrde.github.io

Public site for lorrde's apps, served by GitHub Pages.

| Path | Purpose |
| --- | --- |
| `/cozy-focus/` | Cozy Focus landing page |
| `/cozy-focus/privacy/` | Privacy policy (linked from the app, Google Play and AdMob) |
| `/cozy-focus/auth/` | Where Supabase sends email confirmation links. On Android the app opens these directly (App Links); this page is the fallback with an "Open Cozy Focus" button. |
| `/.well-known/assetlinks.json` | Proves to Android that `io.github.lorrde.cozyfocus` owns the `/cozy-focus/auth/` links |
| `/app-ads.txt` | AdMob publisher verification |
| `/.nojekyll` | Stops GitHub Pages from hiding the `.well-known` folder |

## assetlinks.json fingerprints

Each entry in `sha256_cert_fingerprints` is a signing key allowed to open the links:

- Debug key (builds from the development computer).
- **To add before release:** the "App signing key certificate" SHA-256 from Play Console > Test and release > App integrity.
