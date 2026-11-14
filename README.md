# Sofie Manová – portfolio

Built static site of the portfolio (HTML, CSS, JS and web-optimised photographs), served by
Cloudflare Workers Static Assets at https://sofiamann-webpage.fandlimartin.workers.dev/

- `public/` – the site, exactly as it is served (root-relative paths, base path `/`)
- `wrangler.jsonc` – the Worker: assets only, no server code

Cloudflare Workers Builds deploys this repository on every push to `main` with `npx wrangler deploy`.
This repository holds only the build; it is generated with `npm run build:cloudflare` in the source
project and replaced on each update.
