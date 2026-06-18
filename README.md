# Zumaya Rentals — Demo Site

Concept homepage for **Zumaya Rentals Inc.** (Whittier, CA), intended to be deployed
to `beta.zumayarentals.com` as a private preview before going live.

A single self-contained `index.html` — no build step, no dependencies, no framework.
Just open the file in a browser, or drop it on any static host.

## What's here

- **`index.html`** — the full homepage:
  - Four service lines: Events & Parties, Luxury Restroom Trailers, Production & Film, Dumpsters & Bins
  - Interactive **"Build Your Quote"** catalog (filter, add items, adjust quantities) that feeds the quote form
  - Quote request form (demo preview — see *To do* below)
  - Reviews, Instagram tie-in, consistent name/address/phone

## Local preview

Open `index.html` directly, or serve it:

```bash
python3 -m http.server 8000
# then visit http://localhost:8000
```

## Deploy to beta.zumayarentals.com

1. Push this repo to a static host (Netlify, Vercel, or Cloudflare Pages — all free for this).
2. In the **Namecheap** account that holds `zumayarentals.com`, open **Advanced DNS**.
3. Add a **CNAME** record: host `beta`, value = the address your host gives you.
4. Add `beta.zumayarentals.com` as a custom domain in the host's dashboard.

## To do before launch

- [ ] Replace placeholder photo blocks with Zumaya's real event photos
- [ ] Confirm the correct phone number (site shows 562-903-0858; Yelp shows 562-331-2336)
- [ ] Wire the quote form to a real backend (Netlify Forms / Formspree / CRM) — it's a demo preview right now
- [ ] Confirm the equipment catalog list matches current inventory

## Notes

This is a **private** preview, not the production site. The footer is tagged "DEMO" until launch.
