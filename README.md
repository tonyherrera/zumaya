# Zumaya Rentals — Demo Site

Concept homepage for **Zumaya Rentals Inc.** (Whittier, CA), deployed as a live
team demo at **https://zumaya.vercel.app**.

A static site — no build step, no framework. `index.html` plus an `images/` folder.

## What's here

- **`index.html`** — the full homepage
- **`images/`** — 49 web-optimized equipment photos (from Zumaya's May 2026 price list)

### Features
- Four service lines: Events & Parties, Luxury Restroom Trailers, Production & Film, Dumpsters & Bins
- Interactive **"Build Your Quote"** catalog — 49 real items across 8 categories, with
  real photos and rental pricing (1 day / 2 days / 3 days–weekly)
- Quote request form wired to **Formspree** (`xdavqwon`); the selected equipment list
  rides along in the submission
- Reviews, Instagram tie-in, and the correct name/address/phone block

## Local preview

```bash
python3 -m http.server 8000   # then open http://localhost:8000
```

## Deploy (Vercel)

Already live at zumaya.vercel.app. If the project is linked to GitHub, pushing to the
default branch auto-deploys. To attach a custom domain later, add it under
**Settings → Domains** and create the CNAME Vercel provides in Namecheap.

## Notes / next steps

- [ ] First Formspree submission must be confirmed once (verification email) before leads flow through
- [ ] Pricing reflects the May 2026 list — keep in sync as rates change
- [ ] Optional: add a rental-duration toggle that totals an estimated subtotal
- [ ] Optional: lifestyle/hero photography from real Zumaya events

Pricing source: Zumaya Rentals price list, May 2026. Delivery, services & tax are additional.
