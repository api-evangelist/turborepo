# Turborepo (turborepo)

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

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
