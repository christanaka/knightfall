# create-svelte

Everything you need to build a Svelte project, powered by [`create-svelte`](https://github.com/sveltejs/kit/tree/main/packages/create-svelte).

## Tech

- SvelteKit
- Drizzle ORM
- PostgreSQL
- Tailwind CSS
- Lucia

## Providers

- Neon (PostgreSQL)

## Creating a project

If you're seeing this, you've probably already done this step. Congrats!

```bash
# create a new project in the current directory
npm create svelte@latest

# create a new project in my-app
npm create svelte@latest my-app
```

## Developing

Once you've created a project and installed dependencies with `npm install` (or `pnpm install` or `yarn`), start a development server:

```bash
npm run dev

# or start the server and open the app in a new browser tab
npm run dev -- --open
```

## Drizzle

```bash
# open drizzle studio
pnpm drizzle-kit studio

# generate migration
pnpm drizzle-kit generate:pg

# generate empty migration
drizzle-kit generate:pg --custom

# drop migration
pnpm drizzle-kit drop

# apply migrations
pnpm tsx ./scripts/migrate.ts

# push schema for rapid prototyping
pnpm drizzle-kit push:pg
```

## Building

To create a production version of your app:

```bash
npm run build
```

You can preview the production build with `npm run preview`.

> To deploy your app, you may need to install an [adapter](https://kit.svelte.dev/docs/adapters) for your target environment.

## References

- [Lucia V3 Docs](https://github.com/lucia-auth/lucia/tree/v3/docs)
- [Drizzle Custom Types](https://github.com/drizzle-team/drizzle-orm/blob/main/docs/custom-types.lite.md)
