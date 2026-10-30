<p align="center"><img src=".github/cover.png" alt="Contentrain Astro blog starter — content in Git" width="100%"></p>

> Source of truth: this starter is exported from the `contentrain-starters` monorepo.
> Internal starter id: `astro-blog`.
# Contentrain Astro Blog

Editorial starter for founder letters, product journals, and thoughtful publishing sites.

![Contentrain Astro Blog screenshot](./media/cover.png)

![Contentrain Astro Blog preview](./media/preview.gif)

## Contentrain Ecosystem

Contentrain is a content governance ecosystem for teams and AI agents: content lives in Git as structured JSON and Markdown, agents propose changes, people approve them. This starter keeps every page's content in `.contentrain/` and reads it through a generated, typed SDK client. The ecosystem's other parts: [open-source tools](https://github.com/Contentrain/ai) (MCP, CLI, SDK; MIT), [Studio](https://github.com/Contentrain/studio) for team review and editing, [Migrate](https://migrate.contentrain.io) for moving a WordPress site to Astro, and [Bridge](https://github.com/Contentrain/wordpress-bridge), a free WordPress plugin that exports content as a Contentrain store.

- SDK and CLI: [ai.contentrain.io/packages/sdk](https://ai.contentrain.io/packages/sdk)
- Astro guide: [ai.contentrain.io/guides/frameworks#astro](https://ai.contentrain.io/guides/frameworks#astro)
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
- `pnpm deploy:netlify`
- `pnpm contentrain:generate`

## Demo routes

- `/`
- `/blog/designing-calm-interfaces`
- `/architecture`

## Contentrain

- Seed content lives in `.contentrain/`
- Runtime content queries use the generated `#contentrain` SDK
- Blog pages, navigation, footer, SEO, authors, and categories are content-driven
- The starter follows a git-backed Contentrain architecture so content, schemas, and generated SDK output stay versioned together
- After editing `.contentrain/`, run `pnpm contentrain:generate` to refresh the client
- Prefer Astro content collections? `@contentrain/query/astro` provides `contentrainLoader()`; see the Astro guide

## Deploy

- Netlify build command: `pnpm deploy:netlify`
- Netlify publish directory: `dist`
- `netlify.toml` is committed in the starter root

## Netlify Project Creation

[![Deploy to Netlify](https://www.netlify.com/img/deploy/button.svg)](https://app.netlify.com/start/deploy?repository=https%3A%2F%2Fgithub.com%2FContentrain%2Fcontentrain-starter-astro-blog)

Use `pnpm dlx netlify-cli init` to connect the repository for continuous deployment, or `pnpm dlx netlify-cli link` if the site already exists.

## License

MIT — see [LICENSE](LICENSE).
