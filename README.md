# Sauti Hub

Sauti Hub is an installable podcast-discovery web application. It includes a local podcast collection, YouTube episode playback with automatic queue advance, browser-saved favourites, and live podcast discovery through the public iTunes Search API.

## Run locally

Open the folder through a local web server rather than double-clicking `index.html`. For example, from this folder:

```powershell
npx serve .
```

Then open the localhost address shown by the command.

## Install as an app

The install button appears when the app is hosted on `https://` or `localhost`. Publish this folder to GitHub Pages, Netlify, Vercel, or another HTTPS host. Browsers intentionally do not allow service workers or PWA installation from a `file:///` URL.

## Real services

- Live search uses the public iTunes podcast directory—no client-side API key is stored or required.
- YouTube playback uses the official iframe player API.
- A production LLM assistant, user accounts, email subscriptions, or stored community feedback would need a backend and a protected server-side API key. Do not put those secrets in `index.html`.
