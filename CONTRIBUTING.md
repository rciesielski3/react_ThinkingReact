# Contributing

- Node.js: engines.node >=20.19 required for local development and CI.

Run locally with nvm or volta:

nvm:

```bash
nvm install 20
nvm use 20
npm ci
npm run build
```

volta:

```bash
volta install node@20
npm ci
npm run build
```

Or use Docker with Node 20 image:

```bash
docker run --rm -v "$PWD":/app -w /app node:20 bash -lc "npm ci && npm run build"
```
