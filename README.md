# Crawford County RWD 4 — Utility Portal (Concept Demo)

A working demonstration of an online utility billing and customer portal for
Crawford County Rural Water District No. 4 (Kansas): meter readings entered by
route, automatic bill calculation from the district rate structure, past-due
tracking, and a customer portal with usage history, self-submitted readings,
and simulated online bill pay.

**All data is fictional sample data. No real accounts or payments.**

- Single static file: [`public/index.html`](public/index.html) — no build step,
  no dependencies. Data persists in the browser's localStorage.
- Deployed to Cloudflare Workers (static assets) via `npx wrangler deploy`.

A production version would add Supabase (customer auth + database with
row-level security) and a hosted payment checkout (Stripe / PSN / Municipay)
so card data never touches the district's site.
