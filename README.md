# Pure Baby

A premium baby-care e-commerce **prototype** — baby food, diapers, and skin & bath care.
Single-file React app (React + Babel via CDN), no build step required.

- **Live/preview:** open `index.html` in any browser (needs internet for the React & font CDNs).
- **Brand:** Pure Baby · purebaby.co.in — "Gentle choices for little ones."

## What's inside
Homepage, category pages (Baby Food / Diapers / Skin & Bath), product detail pages,
search, filters & sort, cart + wishlist (localStorage), a prototype checkout (no real
payment), all policy pages, and a WhatsApp CTA. Responsive with a mobile bottom nav and
dark mode.

## Where to change things
Everything lives in `index.html`. Search for these markers:

| Marker | What it controls |
| --- | --- |
| `[CONFIG]` | brand name, WhatsApp number, free-shipping threshold, currency, announcement |
| `[COLORS]` | brand colour system (CSS variables in `:root`) |
| `[LOGO]` | the Pure Baby wordmark component |
| `[DATA]` | the product catalogue (add / edit products) |
| `[IMAGES]` | the placeholder-image layer (swap for licensed assets) |

## Data & disclaimers
Catalogue data is **illustrative prototype data** based on the public MiniMee Kids
catalogue (minimeekids.com): real brands, product names, sizes/packs and diaper weight
ranges; illustrative prices/discounts; ratings shown as "No reviews yet". Long-form copy
and specifications are placeholders — always verify against product packaging.
The `WHATSAPP_NUMBER` in `[CONFIG]` is a **placeholder** (MiniMee's publicly listed phone);
replace it with Pure Baby's own WhatsApp business number. No real payment is processed.

## Deploy
It's a static site — deploy anywhere that serves static files.

- **Vercel:** `npx vercel deploy --prod` from this folder (serves `index.html` at root).
- **GitHub Pages:** enable Pages on the `main` branch (root).
- **Netlify:** drag the folder into Netlify Drop.

## Convert to production later
Replace the in-file `[DATA]` array and `[IMAGES]` layer with a real backend
(Shopify, WooCommerce, Supabase, Firebase, a REST API, or Postgres) and licensed images.
