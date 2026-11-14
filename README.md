# MW4 DMZ Command Center — Prototype 0.1

## Contents
- `index.html`: mobile-first companion app
- `data.json`: editable seed data and source links
- `manifest.json`: installable web-app metadata
- `sw.js`: offline cache for a hosted PWA

## Use immediately
Open `index.html` in a modern browser. Loot, recipes, objectives and notes save in that browser using local storage. Use **Data & Share → Export** to back up or move progress.

## Install and share
For install prompts and offline caching, host this folder on an HTTPS static host (GitHub Pages, Netlify, etc.). Open the hosted URL in Android Chrome and choose Install app / Add to Home screen. Share the hosted URL with your squad.

## Edit
Edit `data.json` to update seed locations, items and sources. Edit `index.html` for interface behavior. Bump the cache name in `sw.js` when publishing an update.

## Important limitations
This is a starter companion, not a verified complete MW4 DMZ database. Recipe, loot-spawn, key, mission, boss and upgrade records must be populated and checked against current game evidence. Map tab currently provides a searchable POI index and links to external interactive maps; exact in-app map pins/coordinates are not bundled. Screenshot analysis prepares a prompt; attach the screenshot in GPT, Claude or Gemini to perform vision analysis. No game memory access, telemetry, live player tracking or AI API integration is implemented. Do not put private API keys in browser code.

## Data verification
Each record should eventually carry source, verification status, game version, map/POI and last-checked date. Prefer official Activision sources; label community reports as such.
