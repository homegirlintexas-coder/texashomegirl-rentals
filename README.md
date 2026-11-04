# Texas HomeGirl — Voucher-Friendly Rentals

Live rental listings page for Texas HomeGirl (Shyanne Johnson, REKonnection LLC).

- `index.html` — the whole site, self-contained (styles, listings data and the Tour & Apply form are all inside it)
- `netlify.toml` — Netlify build settings (no build step; publishes the repo root)

## Updating listings

Listing data lives in the `LISTINGS` array near the bottom of `index.html`.
Each entry: listing id, bedrooms, city, ZIP, monthly rent, note tags, and photo URLs.

Source of truth is NTREIS Matrix. The usual loop:
1. Run the saved lease search in Matrix (agent IDs below), export the results.
2. Update `index.html` from the export.
3. Commit and push — Netlify redeploys automatically.

Partner agent MLS IDs:
`0791459,0693416,0784093,0469575,0690018,0599316`
(Shyanne Johnson, Sebastian Abraham, Pria Bharwani, Carl Anku, Ankit Oberoi, Trecy Phan)
