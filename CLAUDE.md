# Project guide

React 19 + TypeScript + Vite single-page app.

## Commands

- `npm run dev` — start the dev server
- `npm run check` — lint + format check + typecheck + tests (run before considering work done)
- `npm run test` — run tests once (`test:watch` for watch mode)
- `npm run lint:fix` / `npm run format` — auto-fix lint and formatting issues
- `npm run build` — typecheck and produce a production build

## Conventions

- Source lives in `src/`. Import from it with the `@/` alias (e.g. `import Button from '@/components/Button'`).
- Tests are colocated with the code they cover as `*.test.ts(x)`, using Vitest + React Testing Library. Query by role/label, not test IDs, when possible.
- Formatting is Prettier (no semicolons, single quotes) — don't hand-format, run `npm run format`.
- TypeScript is strict; don't suppress errors with `any` or `@ts-ignore` without a comment explaining why.
