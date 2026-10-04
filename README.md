# patrick

Personal website built with Astro and deployed to Cloudflare Workers Static Assets at https://patrick.pe.

Astro generates complete HTML at build time. The pages ship no browser JavaScript and work with JavaScript disabled. Edit the homepage in `src/pages/index.astro` and shared styling in `src/assets/main.css`. Favicons live in `public/`.

## Development

```sh
npm ci
npm run dev
```

Use the local URL printed by Astro. The Astro VS Code extension is recommended for `.astro` files.

## Checks and production build

```sh
npm run lint
npm run build
```

`lint` checks Astro/TypeScript diagnostics and formatting. `npm run format` formats the project. `build` runs Astro checks and generates static HTML and CSS in `dist/`. The footer year is evaluated during the build; rebuild to update it after New Year.

## Cloudflare preview and deployment

```sh
npm run preview
npm run deploy
```

`preview` builds and serves `dist/` locally using Wrangler. `deploy` checks, builds, and uploads those assets to the existing `patrick` Worker and `patrick.pe` custom domain; Cloudflare authentication is required. There is no server-rendering adapter or Worker application script. Unknown URLs use `dist/404.html` with HTTP status 404.
