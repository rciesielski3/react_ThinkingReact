# Changelog

All notable changes to this repository related to dependency upgrades and CI updates.

## 2026-08-13 — Dependency and CI updates
- Bumped `nanoid` to `3.3.17` (security fix for infinite loop when size=0).
- Upgraded `esbuild` to `0.28.2` to satisfy Vite peer requirements and address path traversal advisory on Windows.
- Upgraded `vite` to v8 (validated in Node 20 CI).
- Regenerated `package-lock.json` to match `package.json` and fix `npm ci` in CI.
- Added a Node-20 CI workflow and validated a smoke build on Node 20.
- Bumped/pinned related dev dependencies (`@vitejs/plugin-react`, `rollup`, `postcss`, `@babel/core`) as required for Vite upgrade.

Notes:
- CI now validates on Node 20 (workflow added). Local development may require Node >=20.19.
- If you need to reproduce CI locally, use Docker `node:20` image or switch Node via `nvm`/`volta`.
