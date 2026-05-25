# Turborepo

Turborepo is a high-performance build system for JavaScript and TypeScript monorepos, built by Vercel and written in Rust. It orchestrates task pipelines across a monorepo, hashes task inputs, and caches outputs locally and remotely so the same `build`, `lint`, or `test` never runs twice across developers or CI.

This repository is part of the [API Evangelist](https://apievangelist.com) catalog and profiles Turborepo as both an open-source build tool and as the contract behind the open **Turborepo Remote Cache API** specification.

- Homepage: https://turborepo.dev
- Source: https://github.com/vercel/turborepo
- License: MIT
- Latest release: v2.9.14 (May 2026)

## APIs

- **[Turborepo Remote Cache API](openapi/turborepo-remote-cache-api-openapi.yml)** — HTTP interface any remote cache server must implement to be compatible with `turbo`. Endpoints cover artifact upload/download by content hash, batch query, status, and analytics events. Vercel's `api.vercel.com` is the reference implementation; self-hosted servers (`ducktors/turborepo-remote-cache`, `brunojppb/turbo-cache-server`) implement the same contract.

## Key Features

- Task pipeline orchestration with `dependsOn` graphs
- Content-addressable local caching of task outputs
- Remote Caching with a shared artifact store across teammates and CI
- Open Remote Cache HTTP API — self-hostable, vendor-neutral
- Package-manager agnostic — npm, pnpm, Yarn, Bun
- `turbo prune` for minimal monorepo subsets (Docker-friendly)
- `turbo watch` for dependency-aware single-process watching
- `turbo boundaries` for architectural enforcement
- `turbo query` (GraphQL over the monorepo), `turbo ls`, `turbo gen`
- `turbo-ignore` for CI skip-build decisions
- Codemods via `turbo-codemod`
- VS Code extension and ESLint plugin/config
- Telemetry opt-out via `turbo telemetry`

## Catalog Files

- [`apis.yml`](apis.yml) — APIs.json profile for Turborepo
- [`openapi/turborepo-remote-cache-api-openapi.yml`](openapi/turborepo-remote-cache-api-openapi.yml) — Remote Cache API OpenAPI 3.0 spec
