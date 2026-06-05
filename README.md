# Buildkite (buildkite-com)

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
