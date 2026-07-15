# TrendHive Global Enterprises — Website (Phase 1: Home Page)

## What's included in this phase
- Fully working, responsive **Home page** (`index.html`)
- Modular CSS: `theme.css` (design tokens/dark-light vars), `base.css`, `layout.css` (header/footer/nav), `home.css`, `responsive.css`
- Modular JS: `includes.js` (header/footer partials), `theme.js` (dark/light toggle), `utils.js`, `cart.js` (localStorage cart & wishlist — mock, no backend yet), `products.js` (renders product cards from `data/products.json`), `main.js` (nav, live search, countdown, popups, back-to-top, pincode checker)
- 8 sample products in `data/products.json`
- SEO: meta tags, Open Graph tags, JSON-LD structured data, `robots.txt`, `sitemap.xml`
- Cloudflare Pages config: `_headers` (caching + security headers), `_redirects`

## How to preview locally
```
cd trendhive
python3 -m http.server 8080
```
Then open http://localhost:8080

## Deploying to Cloudflare Pages
1. Push this folder to a GitHub repo.
2. In Cloudflare Pages → Create Project → connect the repo.
3. Build command: (none — static site)
4. Build output directory: `/` (project root)
5. Deploy.

## Known placeholders (intentional, flagged for you)
- Product images use `placehold.co` — swap for real product photos.
- Cart/wishlist/newsletter use `localStorage` only — **no real backend yet**. Orders are not actually processed.
- Payment buttons (Razorpay/PhonePe/UPI/Paytm/COD) will be added as UI placeholders in the checkout phase — real payment processing needs server-side integration (Cloudflare Workers) and can't run purely client-side for security reasons.
- Admin panel needs a real backend (Workers + D1) to manage live inventory/orders — flagged for a later phase.

## Next phases (not yet built)
- Phase 2: Shop page, Product Details page, search filters/sorting, cart page
- Phase 3: Checkout flow + payment placeholders, Account pages (mock auth)
- Phase 4: About, Contact, FAQ, Privacy, Terms, Shipping, Return policy pages
- Phase 5: Admin panel (requires real backend — Workers + D1)

Say "continue to Phase 2" when you're ready and I'll build the Shop + Product Details pages next.
