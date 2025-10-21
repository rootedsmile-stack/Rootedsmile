# RootedSmile Store — GitHub Repo (Cloudflare Pages Ready)

This repository contains a **static**, minimal‑maintenance e‑commerce site for RootedSmile.

## 1) Quick Deploy (Cloudflare Pages)
1. Create a new GitHub repo (e.g., `rootedsmile-store`).
2. Upload these files or push via Git.
3. In **Cloudflare Pages** → **Create Project** → **Connect to GitHub** → select the repo.
4. Set:
   - **Framework preset:** None (just static)
   - **Build command:** _None_
   - **Output directory:** `/` (root)
5. Click **Save and Deploy**.

> Stripe checkout uses **Payment Links**. Replace the test link in `products.json` with your **live** link when ready.

## 2) Customize
- Logo: replace `assets/logo-rootedsmile.png`.
- Copy: edit `index.html`, `about.html`, `shipping-returns.html`.
- Products: edit `products.json` (add items; each needs a `stripe_payment_link`).

## 3) Optional (later)
- **Supabase Auth + Google Login:** add an `/account.html` page that uses Supabase Auth UI. No backend changes required.
- **Custom domain:** after your Pages project is live, add your domain in Cloudflare → DNS and Pages → Custom domains.
- **Analytics:** enable Cloudflare Web Analytics (free).

## 4) Maintenance
- It’s static; updates are just content edits.
- No servers, databases, or webhooks required.
- Rotate Stripe links only when products change.

---

Below is the original README for reference.

# RootedSmile Static Store (Finalized Mockup Text)
Multi-product static store with Your Next Store–style hero, RootedSmile branding, and Stripe Payment Links.
## Headline & Copy
**Clean. Simple. ZingFree.**
Discover the natural way to being zing free without herbal based tooth powder. Gentle, effective.
## Files
- index.html – homepage (logo in header, hero chips, search, grid, footer)
- product.html – dynamic product page (?slug=)
- products.json – product catalog (edit/add items)
- styles.css – cream + olive theme
- script.js – loads catalog, renders grid/product
- assets/logo-rootedsmile.png – your uploaded logo
- assets/icon-cart.svg – cart icon (visual)
## Deploy
Connect GitHub repo to Cloudflare Pages.
- Build command: None
- Output directory: /
## Update Stripe Links
Replace each `stripe_payment_link` in `products.json` with your live Payment Link.
