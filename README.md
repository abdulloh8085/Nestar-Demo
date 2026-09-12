# Nestar demo

Next.js 14.2.1, React ^18 (locked to 18.3.1), TypeScript 5.4.5, and the Pages Router.

## Setup

Node.js 18.17 or newer is required. Use Yarn 1.22.22 and keep `yarn.lock` in version control so dependency versions stay reproducible.

```bash
yarn install --frozen-lockfile
yarn dev
```

Open http://localhost:3000. Edit `pages/index.tsx` for the home page and `pages/api/hello.ts` for the example API.

## Checks and production

```bash
yarn typecheck
yarn lint
yarn build
yarn start
```

The Inter and Roboto Mono fonts use `next/font/google`; the first production build requires access to Google Fonts.

Next.js and tooling versions are pinned in `package.json`; React and React DOM allow version 18 updates through `^18`, with exact installed versions recorded in `yarn.lock`. When changing dependencies intentionally, run `yarn install` and commit the updated `yarn.lock`. Use Yarn consistently to avoid conflicting lockfiles.

Configuration uses `next.config.mjs`, which is supported by Next.js 14. The ESLint configuration uses `next/core-web-vitals` with `eslint-config-next` pinned to the same version as Next.js.

[Next.js 14 documentation](https://nextjs.org/docs/14)
