# Productivity App

A lightweight personal productivity PWA. Single static HTML file, no build step, no
backend — all data is stored locally in your browser via `localStorage`.

## Features

- **Today** – daily to-do / task list
- **Meals** – simple meal planning
- **Grocery list** – running shopping list with prices

Installable to your home screen (iOS/Android) thanks to the web manifest and icons.

## Run it locally

It's just static files, so any static server works. From the project root:

```bash
python3 -m http.server 8000
```

Then open <http://localhost:8000>.

Or simply open `index.html` directly in a browser (some PWA features like the
manifest won't fully apply from `file://`, but the app works).

## Deploy (GitHub Pages)

This repo is set up to publish from the `main` branch root.

1. Push to GitHub.
2. In the repo, go to **Settings → Pages**.
3. Under **Build and deployment**, set **Source** to *Deploy from a branch*,
   branch **`main`**, folder **`/ (root)`**, and save.
4. The site publishes at `https://barbarajhunt.github.io/Productivity-App/`.

## Project structure

```
index.html              # the entire app (markup, styles, logic)
manifest.webmanifest    # PWA manifest
icon-192.png            # PWA / home-screen icons
icon-512.png
apple-touch-icon.png
```
