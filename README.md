# Buildkite (buildkite-com)

Buildkite is a hybrid CI/CD platform that pairs a hosted control plane with self-hosted or Buildkite-Hosted agents that run jobs on customer-controlled infrastructure. The platform spans three core products — Pipelines, Test Engine, and Package Registries — and exposes them through a v2 REST API, a Relay-compliant GraphQL API, an Agent API consumed by the open-source Go agent, webhooks, and an official MCP server that surfaces those APIs to AI coding agents.

**URL:** [Visit APIs.json](https://raw.githubusercontent.com/api-evangelist/buildkite-com/refs/heads/main/apis.yml)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=company-api-evangelist&utm_content=repo)

## Tags

 - CI/CD, Continuous Integration, Continuous Delivery, DevOps, Pipelines, Hybrid CI, Build Automation, Test Engine, Package Registries, Agents, GraphQL, REST, MCP, Webhooks

## Timestamps

- **Created:** 2026-05-25
- **Modified:** 2026-05-25

## Products

| Product | Description |
|---|---|
| Pipelines | YAML-defined CI/CD workflows that run on customer-controlled agents or Buildkite Hosted Agents. Clusters and queues route jobs to specific agent pools. |
| Test Engine | Real-time flaky test management, intelligent test splitting, duration-threshold monitors, and per-test analytics. |
| Package Registries | Hosting for npm, PyPI, RubyGems, Maven, Container, Debian, RPM, Terraform, and Helm packages; Enterprise adds SLSA provenance, license checks, and threat scanning. |

## APIs

### Buildkite REST API
Programmatic access to organizations, pipelines, builds, jobs, artifacts, annotations, agents, clusters, queues, agent tokens, teams, pipeline templates, rules, and emojis. Bearer token authentication with scoped API access tokens.

**Human URL:** [https://buildkite.com/docs/apis/rest-api](https://buildkite.com/docs/apis/rest-api)
**Base URL:** `https://api.buildkite.com/v2`

- [Documentation](https://buildkite.com/docs/apis/rest-api)
- [Authentication](https://buildkite.com/docs/apis/managing-api-tokens)
- [OpenAPI](openapi/buildkite-rest-api-openapi.yml)
- [JSON Schema — Pipeline](json-schema/buildkite-pipeline-schema.json)
- [JSON Schema — Build](json-schema/buildkite-build-schema.json)
- [JSON Schema — Agent](json-schema/buildkite-agent-schema.json)
- [JSON-LD](json-ld/buildkite-com-context.jsonld)
- [Naftiko Capability — Pipelines](capabilities/pipelines.yaml)
- [Naftiko Capability — Builds](capabilities/builds.yaml)
- [Naftiko Capability — Agents](capabilities/agents.yaml)

### Buildkite GraphQL API
Relay-compliant GraphQL endpoint returning deeply nested data on organizations, pipelines, builds, jobs, agents, clusters, queues, teams, audit events, suites, and test executions in a single request. Schema introspection supported; Portals enable scoped, schema-filtered access without per-token scopes.

**Human URL:** [https://buildkite.com/docs/apis/graphql-api](https://buildkite.com/docs/apis/graphql-api)
**Base URL:** `https://graphql.buildkite.com/v1`

- [Documentation](https://buildkite.com/docs/apis/graphql-api)
- [GraphQL Cookbook](https://buildkite.com/docs/apis/graphql/graphql-cookbook)
- [Explorer](https://graphql.buildkite.com/explorer)
- [Naftiko Capability — GraphQL](capabilities/graphql-queries.yaml)

### Buildkite Agent API
Backplane consumed by the open-source Buildkite Agent (Go) to register, accept, and finish jobs, upload artifacts, stream logs, and emit cluster autoscaling metrics. Authenticated with Agent Tokens issued per cluster. Public surface includes `/metrics` and `/stacks`; the `agent-edge.buildkite.com` host adds gRPC methods.

**Human URL:** [https://buildkite.com/docs/apis/agent-api](https://buildkite.com/docs/apis/agent-api)
**Base URL:** `https://agent.buildkite.com/v3`

- [Documentation](https://buildkite.com/docs/apis/agent-api)
- [Agent Source (Go)](https://github.com/buildkite/agent)
- [OpenAPI — public subset](openapi/buildkite-agent-api-openapi.yml)
- [Naftiko Capability — Agents](capabilities/agents.yaml)

### Buildkite Webhooks
Outbound notifications for build, job, agent, ping, deployment, and package events across Pipelines, Test Engine, and Package Registries. Verified with the `X-Buildkite-Token` header.

**Human URL:** [https://buildkite.com/docs/apis/webhooks](https://buildkite.com/docs/apis/webhooks)

- [Documentation](https://buildkite.com/docs/apis/webhooks)
- [Notifications](https://buildkite.com/docs/pipelines/integrations/notifications)

### Buildkite MCP Server
Official Model Context Protocol server that surfaces Buildkite REST API resources as MCP tools and toolsets. Available as both a remote endpoint and a local Go binary.

**Human URL:** [https://github.com/buildkite/buildkite-mcp-server](https://github.com/buildkite/buildkite-mcp-server)

- [Source](https://github.com/buildkite/buildkite-mcp-server)
- [Skills for Claude Code & Cursor](https://github.com/buildkite/skills)

## Open Source

| Repository | Description |
|---|---|
| [buildkite/agent](https://github.com/buildkite/agent) | Buildkite Agent — open-source Go toolkit that runs build jobs on any device or network |
| [buildkite/cli](https://github.com/buildkite/cli) | Buildkite command-line interface |
| [buildkite/go-buildkite](https://github.com/buildkite/go-buildkite) | Go client library for the Buildkite REST API |
| [buildkite/go-pipeline](https://github.com/buildkite/go-pipeline) | Go DSL for defining and manipulating Buildkite pipelines |
| [buildkite/pipeline-schema](https://github.com/buildkite/pipeline-schema) | JSON Schema for Buildkite's pipeline YAML format |
| [buildkite/buildkite-mcp-server](https://github.com/buildkite/buildkite-mcp-server) | Official MCP Server for Buildkite |
| [buildkite/skills](https://github.com/buildkite/skills) | Official Buildkite skills for Claude Code and Cursor |
| [buildkite/agent-stack-k8s](https://github.com/buildkite/agent-stack-k8s) | Autoscaling stack of Buildkite Agents on Kubernetes |
| [buildkite/elastic-ci-stack-for-aws](https://github.com/buildkite/elastic-ci-stack-for-aws) | Auto-scaling cluster of build agents in AWS VPC |
| [buildkite/buildkite-agent-scaler](https://github.com/buildkite/buildkite-agent-scaler) | Lambda for scaling agents based on Buildkite metrics |
| [buildkite/cleanroom](https://github.com/buildkite/cleanroom) | Policy-controlled microVM sandboxes for safe, reproducible workloads |
| [buildkite/emojis](https://github.com/buildkite/emojis) | Custom emoji supported by Buildkite |
| [buildkite/docs](https://github.com/buildkite/docs) | Source files for the Buildkite documentation |

## Plans, Rate Limits, and FinOps

- [Plans & Pricing](plans/buildkite-com-plans-pricing.yml) — Personal (free), Pro ($30/active user/month), Enterprise (contract, 30-user minimum), 30-day All Access Trial
- [Rate Limits](rate-limits/buildkite-com-rate-limits.yml) — per-user and org-wide REST limits, GraphQL complexity, webhook backoff, hosted agent concurrency caps
- [FinOps](finops/buildkite-com-finops.yml) — seat, hosted compute, managed test, and registry storage cost categories with showback levers
- [Vocabulary](vocabulary/buildkite-com-vocabulary.yml)
- [Spectral Rules](rules/buildkite-rules.yml)

## Integrations

GitHub, GitLab, Bitbucket; AWS, GCP, Azure; Kubernetes; Terraform; Slack, MS Teams, PagerDuty, Opsgenie, Datadog, Honeycomb, OpenTelemetry; 1Password, HashiCorp Vault, AWS Secrets Manager; Sentry, Rollbar; Snyk, Aikido, Semgrep; Docker Hub, ECR, GCR, GHCR; OIDC and OAuth Token Exchange (RFC 8693) with major identity providers.

## Maintainers

- [Kin Lane](https://apievangelist.com) — info@apievangelist.com
