# Buildkite (buildkite-com)

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

Buildkite is a hybrid CI/CD platform that combines a hosted control plane (pipelines.buildkite.com) with self-hosted or Buildkite-Hosted agents that run jobs on customer-controlled infrastructure. The platform spans three core products — Pipelines, Test Engine, and Package Registries — and exposes them through a v2 REST API, a Relay-compliant GraphQL API at graphql.buildkite.com/v1, an Agent API at agent.buildkite.com/v3 consumed by the open-source Go agent, webhooks, and an official MCP server that surfaces those APIs to AI coding agents. Customers route work to specific agent pools through clusters and queues, define pipelines as YAML with dynamic uploads, and integrate with the major source control, cloud, identity, secrets, and observability vendors.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/buildkite-com/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/buildkite-com/refs/heads/main/apis.yml)

## Scope

- **Position:** Consuming

## Tags

- CI/CD
- Continuous Integration
- Continuous Delivery
- DevOps
- Pipelines
- Hybrid CI
- Build Automation
- Test Engine
- Package Registries
- Agents
- GraphQL
- REST
- MCP
- Webhooks

## Timestamps

- **Created:** 2026-05-25T00:00:00.000Z
- **Modified:** 2026-05-25

## APIs

### Buildkite REST API

Programmatic access to Buildkite Pipelines covering organizations, pipelines, builds, jobs, artifacts, annotations, agents, clusters, queues, agent tokens, teams, pipeline templates, rules, and emojis. Uses Bearer token authentication with scoped API access tokens. Designed to extend, integrate, and automate CI/CD workflows across hybrid infrastructure.

- **Human URL:** [https://buildkite.com/docs/apis/rest-api](https://buildkite.com/docs/apis/rest-api)
- **Base URL:** `https://api.buildkite.com/v2`

#### Tags

- CI/CD
- Continuous Integration
- Continuous Delivery
- Pipelines
- Builds
- Agents

#### Properties

- [Documentation](https://buildkite.com/docs/apis/rest-api)
- [Authentication](https://buildkite.com/docs/apis/managing-api-tokens)
- [OpenAPI](openapi/buildkite-rest-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/buildkite-rest-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/buildkite-rest-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/buildkite-pipeline-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/buildkite-build-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/buildkite-agent-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON-LD](json-ld/buildkite-com-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)

### Buildkite GraphQL API

GraphQL endpoint that returns deeply nested data on organizations, pipelines, builds, jobs, agents, clusters, queues, teams, audit events, suites, test executions, and package registries in a single request. Implements the Relay specification for pagination and supports schema introspection. Requires an API access token with "Enable GraphQL API Access" permission. GraphQL Portals allow scoped, schema-filtered access without per-token scopes.

- **Human URL:** [https://buildkite.com/docs/apis/graphql-api](https://buildkite.com/docs/apis/graphql-api)
- **Base URL:** `https://graphql.buildkite.com/v1`

#### Tags

- CI/CD
- GraphQL
- Pipelines
- Test Engine

#### Properties

- [Documentation](https://buildkite.com/docs/apis/graphql-api)
- [Documentation](https://buildkite.com/docs/apis/graphql/graphql-cookbook)
- [Sandbox](https://graphql.buildkite.com/explorer)
- [Postman Collection](collections/buildkite-agent-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/buildkite-agent-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/buildkite-rest-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/buildkite-rest-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Buildkite Agent API

Backplane consumed by the Buildkite Agent (open source, Go) to register, deregister, accept and finish jobs, upload artifacts, stream job logs, and emit metrics for cluster autoscaling. Authenticated via Agent Tokens issued per cluster. Public surface includes `/metrics` (for autoscaling) and `/stacks` (for self-hosted queue controllers). The `agent-edge.buildkite.com` host adds gRPC methods. Most other endpoints are reserved for internal agent use.

- **Human URL:** [https://buildkite.com/docs/apis/agent-api](https://buildkite.com/docs/apis/agent-api)
- **Base URL:** `https://agent.buildkite.com/v3`

#### Tags

- CI/CD
- Agents
- Hybrid CI

#### Properties

- [Documentation](https://buildkite.com/docs/apis/agent-api)
- [Documentation](https://buildkite.com/docs/agent/v3)
- [Source Code](https://github.com/buildkite/agent)
- [Postman Collection](collections/buildkite-agent-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/buildkite-agent-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/buildkite-rest-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/buildkite-rest-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Buildkite Webhooks

Outbound HTTP notifications fired in response to build, job, agent, ping, deployment, and package events across Pipelines, Test Engine, and Package Registries. Verified with the `X-Buildkite-Token` header. Configured per organization via Notification Services. Supports an expanded set of GitHub-style triggers including pull request reviews, releases, issue comments, and deployment status events.

- **Human URL:** [https://buildkite.com/docs/apis/webhooks](https://buildkite.com/docs/apis/webhooks)

#### Tags

- CI/CD
- Webhooks
- Events
- Notifications

#### Properties

- [Documentation](https://buildkite.com/docs/apis/webhooks)
- [Documentation](https://buildkite.com/docs/pipelines/integrations/notifications)
- [Postman Collection](collections/buildkite-agent-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/buildkite-agent-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/buildkite-rest-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/buildkite-rest-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Buildkite MCP Server

Official Model Context Protocol server that exposes Buildkite REST API surfaces (pipelines, builds, jobs, agents, artifacts, annotations) as MCP tools and toolsets for AI coding agents. Available as both a remote endpoint and a local binary. Pairs with the official Buildkite Skills for Claude Code and Cursor.

- **Human URL:** [https://github.com/buildkite/buildkite-mcp-server](https://github.com/buildkite/buildkite-mcp-server)

#### Tags

- CI/CD
- MCP
- Model Context Protocol
- AI
- Agents

#### Properties

- [Documentation](https://github.com/buildkite/buildkite-mcp-server)
- [Source Code](https://github.com/buildkite/buildkite-mcp-server)
- [Postman Collection](collections/buildkite-agent-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/buildkite-agent-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/buildkite-rest-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/buildkite-rest-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [Arazzo Workflows](arazzo/) — [Arazzo Specification](https://spec.openapis.org/arazzo/latest.html)
- [Portal](https://buildkite.com)
- [Documentation](https://buildkite.com/docs)
- [Getting Started](https://buildkite.com/docs/tutorials/getting-started)
- [Sign Up](https://buildkite.com/signup)
- [Pricing](https://buildkite.com/pricing)
- [Terms of Service](https://buildkite.com/legal/terms-of-service)
- [Privacy Policy](https://buildkite.com/legal/privacy-policy)
- [Security Policy](https://buildkite.com/security)
- [Trust Center](https://buildkite.com/security)
- [Status Page](https://buildkitestatus.com)
- [Changelog](https://buildkite.com/changelog)
- [Blog](https://buildkite.com/blog)
- [Forum](https://forum.buildkite.community)
- [Support](https://buildkite.com/support)
- [Authentication](https://buildkite.com/docs/apis/managing-api-tokens)
- [Rate Limits](https://buildkite.com/docs/apis/rest-api#rate-limits)
- [GitHub Organization](https://github.com/buildkite)
- [Source Code](https://github.com/buildkite/agent)
- [C L I](https://github.com/buildkite/cli)
- [SDK](https://github.com/buildkite/go-buildkite)
- [SDK](https://github.com/buildkite/go-pipeline)
- [JSON Schema](https://github.com/buildkite/pipeline-schema) — [JSON Schema](https://json-schema.org/specification)
- [Tool](https://github.com/buildkite/buildkite-mcp-server)
- [Tool](https://github.com/buildkite/skills)
- [Tool](https://github.com/buildkite/agent-stack-k8s)
- [Tool](https://github.com/buildkite/elastic-ci-stack-for-aws)
- [Tool](https://github.com/buildkite/buildkite-agent-scaler)
- [Tool](https://github.com/buildkite/cleanroom)
- [Tool](https://github.com/buildkite/emojis)
- [Source Code](https://github.com/buildkite/docs)
- [Integrations](undefined)
- [Features](undefined)
- [Plans](plans/buildkite-com-plans-pricing.yml)
- [Rate Limits](rate-limits/buildkite-com-rate-limits.yml)
- [Fin Ops](finops/buildkite-com-finops.yml)
- [Vocabulary](vocabulary/buildkite-com-vocabulary.yml)
- [Spectral Rules](rules/buildkite-rules.yml) — [Spectral](https://docs.stoplight.io/docs/spectral)

## Maintainers

**FN:** Kin Lane
**Email:** info@apievangelist.com
**URL:** https://apievangelist.com
