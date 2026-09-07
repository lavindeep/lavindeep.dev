# lavindeep.dev

Personal site. One static HTML file in `public/`, no build step, no dependencies.

## Run locally

    python3 -m http.server 8000 -d public

Then open http://localhost:8000.

## Deploy

Cloudflare Workers serves `public/` as static assets, configured in `wrangler.jsonc`.
Every push to `main` deploys via `npx wrangler deploy`.
