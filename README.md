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

## Stock indicators

Add `st` to any item in the `ITEMS` array:
- `st: 0` → "Tükendi / Нет в наличии", ordering disabled
- `st: 1–5` → "Son X / Осталось X" badge, cart quantity capped at X
- no `st` field → normal availability, no badge

Example: `{c:"cakes", t:"Napoleon", r:"Торт «Наполеон»", p:1200, u:"kg", st: 2},`

## Editing products

All products live in `index.html` inside the `ITEMS` array (TR/RU names, price, unit, category).
Product photos are mapped by TR name in the `IMGS` object — replace any URL with the client's own photo.
