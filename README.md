# Vkusno Homemade — Ankara

Online store for Vkusno Homemade (Azerbaijani, Russian & Uzbek homestyle food, Çankaya/Ankara).
Single-page site with product catalog, cart, TR/RU languages and WhatsApp checkout.

## Run locally

Open `index.html` in a browser, or:

```bash
npm install
npm start
```

## Deploy (Railway)

Railway auto-detects Node via `package.json` and runs `npm start` (static server on `$PORT`).

## Editing products

All products live in `index.html` inside the `ITEMS` array (TR/RU names, price, unit, category).
Product photos are mapped by TR name in the `IMGS` object — replace any URL with the client's own photo.
