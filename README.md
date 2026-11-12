# RK's Drink Library

A mobile-first, installable drink library and **Whiskey Powers** batch calculator. No build step.

## Add to Home Screen (iPhone)

1. Open the site in Safari.
2. Tap the Share button, then **Add to Home Screen**.

After the first visit it works offline. The app has three tabs: a searchable card library, a Surprise me shaker, and the batch calculator.

## Run locally

```bash
python3 -m http.server 8080
```

Then visit `http://localhost:8080`.

Drinks live in [`drinks.json`](drinks.json). Add or edit entries there; the page loads that file.

Each drink object looks like:

```json
{
  "name": "Whiskey Powers",
  "spirit": "Bourbon",
  "ingredients": "Maker's Mark bourbon, jalapeño agave, lime, cinnamon, vanilla, egg white",
  "type": "Seasonal",
  "price": 14,
  "source": "Bar menu photo, Oct 10, 2026",
  "notes": "Optional tasting or recipe notes."
}
```

The starting ten drinks are from a bar menu photo dated Oct 10, 2026.
