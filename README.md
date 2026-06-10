# react-vite-ts-template

A starter template for React projects:

- ⚛️ [React 19](https://react.dev/) + [TypeScript](https://www.typescriptlang.org/) (strict mode)
- ⚡ [Vite 8](https://vite.dev/) for dev server and builds
- 🧹 [ESLint](https://eslint.org/) (flat config) + [Prettier](https://prettier.io/), wired together via `eslint-config-prettier`
- 🧪 [Vitest](https://vitest.dev/) + [React Testing Library](https://testing-library.com/docs/react-testing-library/intro/) with jsdom and jest-dom matchers
- 🤖 GitHub Actions CI: lint, format check, tests, and build on every push/PR to `main`
- 🛠️ `@/` import alias for `src/`, `.editorconfig`, `.nvmrc`, VS Code settings, and a `CLAUDE.md` for working with Claude Code

## Using this template

On GitHub, click **Use this template**, or clone it locally:

```sh
npx degit <your-username>/react-vite-ts-template my-app
cd my-app
npm install
```

Then update the `name` field in `package.json` and the `<title>` in `index.html`.

## Scripts

| Command                 | Description                             |
| ----------------------- | --------------------------------------- |
| `npm run dev`           | Start the dev server with HMR           |
| `npm run build`         | Typecheck and build for production      |
| `npm run preview`       | Preview the production build locally    |
| `npm run test`          | Run tests once                          |
| `npm run test:watch`    | Run tests in watch mode                 |
| `npm run test:coverage` | Run tests with a coverage report        |
| `npm run lint`          | Lint with ESLint                        |
| `npm run lint:fix`      | Lint and auto-fix                       |
| `npm run format`        | Format everything with Prettier         |
| `npm run format:check`  | Check formatting without writing        |
| `npm run typecheck`     | Typecheck without emitting              |
| `npm run check`         | Lint + format check + typecheck + tests |

## Notes

- Node version is pinned to 24 LTS in `.nvmrc` (`nvm use` to switch). Anything `>=20.19` works.
- Tests are colocated with source files as `*.test.ts(x)`; shared setup lives in `src/setupTests.ts`.
- Import from `src/` anywhere with the `@/` alias, configured in both `vite.config.ts` and `tsconfig.app.json`.
