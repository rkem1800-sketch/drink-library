# RK's Drink Library

A small static site for saving drinks from bar menus and batching **Whiskey Powers** at home.

Open the live site, or serve this folder locally:

```bash
python3 -m http.server 8080
```

Then visit `http://localhost:8080`.

## What's in it

- **Drink Library** — searchable list of saved drinks (name, ingredients, notes) with spirit and type filters.
- **Whiskey Powers Calculator** — enter a headcount and heat level (mild / medium / hot) to get quantities, a Harris Teeter Sun Valley shopping list, the jalapeño agave syrup recipe, and a two-at-a-time shaking plan.

Drinks live in [`drinks.json`](drinks.json). Add or edit entries there; the page loads that file. There is no build step and no external network dependencies.

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
