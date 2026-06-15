# Turborepo (turborepo)

Turborepo is a high-performance build system for JavaScript and TypeScript codebases, built by Vercel and written in Rust. It accelerates monorepo development by orchestrating task pipelines with explicit dependency graphs, hashing task inputs to skip redundant work, and caching task outputs locally and remotely so the same build/lint/test never runs twice across developers and CI. The project ships the turbo CLI (turbo run, prune, watch, boundaries, ls, query, generate, login, link, telemetry) plus an open Remote Cache HTTP API specification that any server can implement — Vercel's Remote Cache is the reference, and community implementations enable fully self-hosted caching. Turborepo is MIT-licensed open source at github.com/vercel/turborepo.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/turborepo/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/turborepo/refs/heads/main/apis.yml)

## Scope

- **Position:** Consuming
- **Access:** 3rd-Party

## Tags

- Build System
- Monorepo
- JavaScript
- TypeScript
- Caching
- Open Source
- Rust
- Vercel
- Developer Tools
- CI/CD

## Timestamps

- **Created:** 2026-05-25T00:00:00.000Z
- **Modified:** 2026-05-25

## APIs

### Turborepo Remote Cache API

The Turborepo Remote Cache API specification defines the HTTP interface that any remote cache server must implement to be compatible with Turborepo. The remote cache stores build artifacts (outputs from tasks like build, lint, test) identified by content-addressable hashes. Endpoints cover artifact upload (PUT /artifacts/{hash}), download (GET /artifacts/{hash}), existence checks (HEAD), batch queries (POST /artifacts), status (/artifacts/status), and analytics events (POST /artifacts/events). The Vercel Remote Cache at api.vercel.com is the reference implementation; teams may self-host their own remote cache server (e.g. ducktors/ turborepo-remote-cache).

- **Human URL:** [https://turborepo.dev/docs/core-concepts/remote-caching](https://turborepo.dev/docs/core-concepts/remote-caching)

#### Tags

- Build System
- Caching
- Monorepo
- Remote Cache
- Artifacts

#### Properties

- [Documentation](https://turborepo.dev/docs/core-concepts/remote-caching)
- [Documentation](https://turborepo.dev/docs/openapi)
- [OpenAPI](https://turborepo.dev/api/remote-cache-spec) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [OpenAPI](openapi/turborepo-remote-cache-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/turborepo-remote-cache-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/turborepo-remote-cache-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [Portal](https://turborepo.dev)
- [Documentation](https://turborepo.dev/docs)
- [Getting Started](https://turborepo.dev/docs/getting-started/installation)
- [Documentation](https://turborepo.dev/docs/reference/configuration)
- [Documentation](https://turborepo.dev/docs/reference)
- [Documentation](https://turborepo.dev/docs/core-concepts/remote-caching)
- [Documentation](https://turborepo.dev/docs/crafting-your-repository)
- [Documentation](https://turborepo.dev/docs/telemetry)
- [Blog](https://turborepo.dev/blog)
- [Documentation](https://turborepo.dev/showcase)
- [GitHub Organization](https://github.com/vercel/turborepo)
- [Source Code](https://github.com/vercel/turborepo)
- [Changelog](https://github.com/vercel/turborepo/releases)
- [License](https://github.com/vercel/turborepo/blob/main/LICENSE)
- [Security Policy](https://github.com/vercel/turborepo/blob/main/SECURITY.md)
- [Code Of Conduct](https://github.com/vercel/turborepo/blob/main/CODE_OF_CONDUCT.md)
- [Documentation](https://github.com/vercel/turborepo/blob/main/CONTRIBUTING.md)
- [Package](https://www.npmjs.com/package/turbo)
- [Package](https://www.npmjs.com/package/create-turbo)
- [Package](https://www.npmjs.com/package/eslint-config-turbo)
- [Package](https://www.npmjs.com/package/eslint-plugin-turbo)
- [Package](https://www.npmjs.com/package/turbo-ignore)
- [Code Examples](https://github.com/vercel/turborepo/tree/main/examples)
- [Documentation](https://vercel.com/docs/monorepos/turborepo)
- [Documentation](https://vercel.com/docs/monorepos/remote-caching)
- [Pricing](https://vercel.com/pricing)
- [Authentication](https://vercel.com/account/tokens)
- [Forum](https://github.com/vercel/turborepo/discussions)
- [X (Twitter)](https://x.com/turborepo)
- [Blue Sky](https://bsky.app/profile/turborepo.com)
- [Features](undefined)

## Maintainers

**FN:** Kin Lane
**Email:** info@apievangelist.com
**URL:** https://apievangelist.com
