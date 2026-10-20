# Cronbeat Web

React client for [Cronbeat](https://github.com/moistrenko/cronbeat-api), a dead man's switch for scheduled jobs. A cron task pings a unique URL when it finishes. If the ping does not arrive on time, Cronbeat sends an alert.

This repository is the single-page application. The Laravel API lives in [cronbeat-api](https://github.com/moistrenko/cronbeat-api).

The UI is the Vite starter screen. Dashboard, forms, and API calls are not built yet.

## Requirements

- Node.js 22 or newer
- pnpm

## Local setup

```bash
pnpm install
pnpm dev
```

The dev server runs at http://localhost:5173.

## Checks

```bash
pnpm typecheck
pnpm lint
pnpm format
pnpm build
```

`typecheck` runs `tsc` without emitting files. Vite does not typecheck during `pnpm dev`. `lint` runs ESLint. `format` rewrites sources with Prettier (4-space indent, LF). `build` typechecks and then produces `dist/`.

Do not commit `node_modules/` or `dist/`.
