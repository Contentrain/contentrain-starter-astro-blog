> Source of truth: this starter is exported from the `contentrain-starters` monorepo.
> Internal starter id: `astro-blog`.
# Contentrain Astro Blog

Editorial starter for founder letters, product journals, and thoughtful publishing sites.

## Contentrain Ecosystem

- SDK and CLI: [ai.contentrain.io/packages/sdk.html](https://ai.contentrain.io/packages/sdk.html)
- Product guides: [docs.contentrain.io](https://docs.contentrain.io/)
- Editorial and content operations UI: [studio.contentrain.io](https://studio.contentrain.io)

## Quick Start

```bash
pnpm install
pnpm dev
```

## Commands

- `pnpm dev`
- `pnpm check`
- `pnpm build`
- `pnpm preview`
- `pnpm contentrain:generate`

## Contentrain

- Seed content lives in `.contentrain/`
- Runtime content queries use the generated `#contentrain` SDK
- Blog pages, navigation, footer, SEO, authors, and categories are content-driven
- The starter follows a git-backed Contentrain architecture so content, schemas, and generated SDK output stay versioned together

## Deploy

- Vercel: `pnpm deploy:vercel`
- Netlify: `pnpm deploy:netlify`
- Cloudflare Pages: `pnpm deploy:cloudflare`
- Static output directory: `dist`
