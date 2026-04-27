# Disgrace

Psychological horror containment prototype built as a single static site.

## GitHub Pages Ready

This project can be deployed directly to GitHub Pages because it only needs:

- `index.html`
- `404.html`
- `site.webmanifest`
- `firebase-config.js`

If Firebase is not configured, the game runs locally with browser storage only.
If `localStorage` is blocked, it falls back to `sessionStorage`, then to in-memory storage for the current tab.

## Optional Firebase Setup

Remote save sync is optional. To enable it, edit [firebase-config.js](./firebase-config.js) and replace the default `null` value with your Firebase web config object.

Recommended Firebase features:

- Anonymous Authentication
- Email/Password Authentication
- Firestore
- Realtime Database

The game will try to use Firestore and Realtime Database when available. Players can create an optional account to sync progress, but signing in is never required. If remote auth or sync fails, the game falls back to local-only guest mode without blocking gameplay.

## Deploying To GitHub Pages

1. Push this repository to GitHub.
2. Open `Settings` -> `Pages`.
3. Set the source to deploy from your default branch root.
4. Wait for GitHub Pages to publish the site.

Because all asset paths are relative, it is safe to host this from a repository subpath such as `https://username.github.io/Disgrace/`.
The included `404.html` redirects stray GitHub Pages requests back to `index.html` so accidental deep links fail more gracefully.
