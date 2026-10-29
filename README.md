# Buildkite

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

**Areas:** CI/CD · Continuous Integration · Continuous Delivery · DevOps · Pipelines · Hybrid CI · Build Automation · Test Engine · Package Registries · Agents · GraphQL · REST

## Buildkite on APIs.io

Everything profiled for Buildkite is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/buildkite-com/](https://apis.io/providers/buildkite-com/)** — or go straight to one of the APIs or properties below.

### APIs (23)

- [Buildkite GraphQL API](https://apis.io/apis/buildkite-com/buildkite-graphql-api/) — GraphQL endpoint that returns deeply nested data on organizations, pipelines, builds, jobs, agents, clusters, queues, teams, audit events, suites, test…
- [Buildkite Agent API](https://apis.io/apis/buildkite-com/buildkite-agent-api/) — Backplane consumed by the Buildkite Agent (open source, Go) to register, deregister, accept and finish jobs, upload artifacts, stream job logs, and emit…
- [Buildkite Webhooks](https://apis.io/apis/buildkite-com/buildkite-webhooks/) — Outbound HTTP notifications fired in response to build, job, agent, ping, deployment, and package events across Pipelines, Test Engine, and Package…
- [Buildkite MCP Server](https://apis.io/apis/buildkite-com/buildkite-mcp-server/) — Official Model Context Protocol server that exposes Buildkite REST API surfaces (pipelines, builds, jobs, agents, artifacts, annotations) as MCP tools and…
- [Buildkite Access Token API](https://apis.io/apis/buildkite-com/buildkite-com-access-token-api/) — The Access Token API from Buildkite — 1 operation(s) for access token.
- [Buildkite Agent Tokens API](https://apis.io/apis/buildkite-com/buildkite-com-agent-tokens-api/) — The Agent Tokens API from Buildkite — 1 operation(s) for agent tokens.
- [Buildkite Agents API](https://apis.io/apis/buildkite-com/buildkite-com-agents-api/) — The Agents API from Buildkite — 3 operation(s) for agents.
- [Buildkite Annotations API](https://apis.io/apis/buildkite-com/buildkite-com-annotations-api/) — The Annotations API from Buildkite — 1 operation(s) for annotations.
- [Buildkite Artifacts API](https://apis.io/apis/buildkite-com/buildkite-com-artifacts-api/) — The Artifacts API from Buildkite — 1 operation(s) for artifacts.
- [Buildkite Builds API](https://apis.io/apis/buildkite-com/buildkite-com-builds-api/) — The Builds API from Buildkite — 4 operation(s) for builds.
- [Buildkite Clusters API](https://apis.io/apis/buildkite-com/buildkite-com-clusters-api/) — The Clusters API from Buildkite — 1 operation(s) for clusters.
- [Buildkite Emojis API](https://apis.io/apis/buildkite-com/buildkite-com-emojis-api/) — The Emojis API from Buildkite — 1 operation(s) for emojis.
- [Buildkite Jobs API](https://apis.io/apis/buildkite-com/buildkite-com-jobs-api/) — The Jobs API from Buildkite — 2 operation(s) for jobs.
- [Buildkite Meta API](https://apis.io/apis/buildkite-com/buildkite-com-meta-api/) — The Meta API from Buildkite — 1 operation(s) for meta.
- [Buildkite Metrics API](https://apis.io/apis/buildkite-com/buildkite-com-metrics-api/) — The Metrics API from Buildkite — 1 operation(s) for metrics.
- [Buildkite Organizations API](https://apis.io/apis/buildkite-com/buildkite-com-organizations-api/) — The Organizations API from Buildkite — 2 operation(s) for organizations.
- [Buildkite Pipeline Templates API](https://apis.io/apis/buildkite-com/buildkite-com-pipeline-templates-api/) — The Pipeline Templates API from Buildkite — 1 operation(s) for pipeline templates.
- [Buildkite Pipelines API](https://apis.io/apis/buildkite-com/buildkite-com-pipelines-api/) — The Pipelines API from Buildkite — 2 operation(s) for pipelines.
- [Buildkite Queues API](https://apis.io/apis/buildkite-com/buildkite-com-queues-api/) — The Queues API from Buildkite — 1 operation(s) for queues.
- [Buildkite Rules API](https://apis.io/apis/buildkite-com/buildkite-com-rules-api/) — The Rules API from Buildkite — 1 operation(s) for rules.
- [Buildkite Stacks API](https://apis.io/apis/buildkite-com/buildkite-com-stacks-api/) — The Stacks API from Buildkite — 1 operation(s) for stacks.
- [Buildkite Teams API](https://apis.io/apis/buildkite-com/buildkite-com-teams-api/) — The Teams API from Buildkite — 1 operation(s) for teams.
- [Buildkite User API](https://apis.io/apis/buildkite-com/buildkite-com-user-api/) — The User API from Buildkite — 1 operation(s) for user.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### Arazzo workflows (9)

Multi-step workflows that chain operations into a business task.

- [Buildkite Build Failure Triage](https://apis.io/arazzos/buildkite-com/buildkite-com-build-failure-triage-workflow/)
- [Buildkite Cancel Running Build](https://apis.io/arazzos/buildkite-com/buildkite-com-cancel-running-build-workflow/)
- [Buildkite Collect Build Artifacts](https://apis.io/arazzos/buildkite-com/buildkite-com-collect-build-artifacts-workflow/)
- [Buildkite Fetch Job Log](https://apis.io/arazzos/buildkite-com/buildkite-com-fetch-job-log-workflow/)
- [Buildkite Provision Pipeline And First Build](https://apis.io/arazzos/buildkite-com/buildkite-com-provision-pipeline-and-first-build-workflow/)
- [Buildkite Rebuild Latest Build](https://apis.io/arazzos/buildkite-com/buildkite-com-rebuild-latest-build-workflow/)
- [Buildkite Retry Failed Job](https://apis.io/arazzos/buildkite-com/buildkite-com-retry-failed-job-workflow/)
- [Buildkite Stop Disconnected Agent](https://apis.io/arazzos/buildkite-com/buildkite-com-stop-disconnected-agent-workflow/)
- [Buildkite Trigger And Poll Build](https://apis.io/arazzos/buildkite-com/buildkite-com-trigger-and-poll-build-workflow/)

#### AsyncAPI (1)

Event-driven and webhook contracts.

- [Buildkite Com Webhooks](https://apis.io/asyncapis/buildkite-com/buildkite-com-webhooks/)

#### GraphQL (1)

GraphQL schemas.

- [Buildkite GraphQL API](https://apis.io/graphqls/buildkite-com/buildkite-com-graphql/)

#### MCP servers (1)

Model Context Protocol servers that expose the API to agents.

- [buildkite](https://apis.io/servers/buildkite-com/buildkite/)

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Buildkite Com Agentic Access](https://apis.io/agentic-access/buildkite-com/buildkite-com-agentic-access/)

#### JSON Schema (3)

The data models the API reads and writes.

- [Buildkite Agent](https://apis.io/schemas/buildkite-com/buildkite-agent/)
- [Buildkite Build](https://apis.io/schemas/buildkite-com/buildkite-build/)
- [Buildkite Pipeline](https://apis.io/schemas/buildkite-com/buildkite-pipeline/)

#### JSON Structure (1)

Data models expressed in JSON Structure.

- [Buildkite Com Pipeline Structure](https://apis.io/json-structure/buildkite-com/buildkite-com-pipeline-structure/)

#### JSON-LD (1)

Linked-data contexts for the provider's vocabulary.

- [Buildkite Com Context](https://apis.io/jsonld/buildkite-com/buildkite-com-context/)

#### Vocabulary (1)

The provider's domain terms, defined.

- [Buildkite Com Vocabulary](https://apis.io/vocabularies/buildkite-com/buildkite-com-vocabulary/)

#### Examples (3)

Example requests and responses.

- [Buildkite Create Build Example](https://apis.io/examples/buildkite-com/buildkite-create-build-example/)
- [Buildkite Graphql Builds Example](https://apis.io/examples/buildkite-com/buildkite-graphql-builds-example/)
- [Buildkite List Agents Example](https://apis.io/examples/buildkite-com/buildkite-list-agents-example/)

#### Collections (22)

Postman and Open Collection request collections.

- [Buildkite Agent API](https://apis.io/collections/buildkite-com/open-buildkite-agent-api/)
- [Buildkite Agent Access Token API](https://apis.io/collections/buildkite-com/open-buildkite-com-access-token-api/)
- [Buildkite Agent Access Token Agent Tokens API](https://apis.io/collections/buildkite-com/open-buildkite-com-agent-tokens-api/)
- [Buildkite Agent Access Token Agents API](https://apis.io/collections/buildkite-com/open-buildkite-com-agents-api/)
- [Buildkite Agent Access Token Annotations API](https://apis.io/collections/buildkite-com/open-buildkite-com-annotations-api/)
- [Buildkite Agent Access Token Artifacts API](https://apis.io/collections/buildkite-com/open-buildkite-com-artifacts-api/)
- [Buildkite Agent Access Token Builds API](https://apis.io/collections/buildkite-com/open-buildkite-com-builds-api/)
- [Buildkite Agent Access Token Clusters API](https://apis.io/collections/buildkite-com/open-buildkite-com-clusters-api/)
- [Buildkite Agent Access Token Emojis API](https://apis.io/collections/buildkite-com/open-buildkite-com-emojis-api/)
- [Buildkite Agent Access Token Jobs API](https://apis.io/collections/buildkite-com/open-buildkite-com-jobs-api/)
- [Buildkite Agent Access Token Meta API](https://apis.io/collections/buildkite-com/open-buildkite-com-meta-api/)
- [Buildkite Agent Access Token Metrics API](https://apis.io/collections/buildkite-com/open-buildkite-com-metrics-api/)
- [Buildkite Agent Access Token Organizations API](https://apis.io/collections/buildkite-com/open-buildkite-com-organizations-api/)
- [Buildkite Agent Access Token Pipeline Templates API](https://apis.io/collections/buildkite-com/open-buildkite-com-pipeline-templates-api/)
- [Buildkite Agent Access Token Pipelines API](https://apis.io/collections/buildkite-com/open-buildkite-com-pipelines-api/)
- [Buildkite Agent Access Token Queues API](https://apis.io/collections/buildkite-com/open-buildkite-com-queues-api/)
- [Buildkite Agent Access Token Rules API](https://apis.io/collections/buildkite-com/open-buildkite-com-rules-api/)
- [Buildkite Agent Access Token Stacks API](https://apis.io/collections/buildkite-com/open-buildkite-com-stacks-api/)
- [Buildkite Agent Access Token Teams API](https://apis.io/collections/buildkite-com/open-buildkite-com-teams-api/)
- [Buildkite Agent Access Token User API](https://apis.io/collections/buildkite-com/open-buildkite-com-user-api/)
- [Buildkite REST API](https://apis.io/collections/buildkite-com/open-buildkite-rest-api/)
- [Buildkite REST API](https://apis.io/collections/buildkite-com/postman-buildkite-rest-api/)

#### Overlays (22)

OpenAPI overlays, including conversational phrasing for each operation.

- [Buildkite Com Access Token Api Phrasing Overlay](https://apis.io/overlays/buildkite-com/buildkite-com-access-token-api-phrasing-overlay/)
- [Buildkite Com Agent Api Overlay](https://apis.io/overlays/buildkite-com/buildkite-com-agent-api-overlay/)
- [Buildkite Com Agent Tokens Api Phrasing Overlay](https://apis.io/overlays/buildkite-com/buildkite-com-agent-tokens-api-phrasing-overlay/)
- [Buildkite Com Agents Api Overlay](https://apis.io/overlays/buildkite-com/buildkite-com-agents-api-overlay/)
- [Buildkite Com Agents Api Phrasing Overlay](https://apis.io/overlays/buildkite-com/buildkite-com-agents-api-phrasing-overlay/)
- [Buildkite Com Annotations Api Phrasing Overlay](https://apis.io/overlays/buildkite-com/buildkite-com-annotations-api-phrasing-overlay/)
- [Buildkite Com Artifacts Api Phrasing Overlay](https://apis.io/overlays/buildkite-com/buildkite-com-artifacts-api-phrasing-overlay/)
- [Buildkite Com Builds Api Phrasing Overlay](https://apis.io/overlays/buildkite-com/buildkite-com-builds-api-phrasing-overlay/)
- [Buildkite Com Clusters Api Phrasing Overlay](https://apis.io/overlays/buildkite-com/buildkite-com-clusters-api-phrasing-overlay/)
- [Buildkite Com Emojis Api Phrasing Overlay](https://apis.io/overlays/buildkite-com/buildkite-com-emojis-api-phrasing-overlay/)
- [Buildkite Com Jobs Api Phrasing Overlay](https://apis.io/overlays/buildkite-com/buildkite-com-jobs-api-phrasing-overlay/)
- [Buildkite Com Meta Api Phrasing Overlay](https://apis.io/overlays/buildkite-com/buildkite-com-meta-api-phrasing-overlay/)
- [Buildkite Com Metrics Api Phrasing Overlay](https://apis.io/overlays/buildkite-com/buildkite-com-metrics-api-phrasing-overlay/)
- [Buildkite Com Organizations Api Phrasing Overlay](https://apis.io/overlays/buildkite-com/buildkite-com-organizations-api-phrasing-overlay/)
- [Buildkite Com Pipeline Templates Api Phrasing Overlay](https://apis.io/overlays/buildkite-com/buildkite-com-pipeline-templates-api-phrasing-overlay/)
- [Buildkite Com Pipelines Api Phrasing Overlay](https://apis.io/overlays/buildkite-com/buildkite-com-pipelines-api-phrasing-overlay/)
- [Buildkite Com Queues Api Phrasing Overlay](https://apis.io/overlays/buildkite-com/buildkite-com-queues-api-phrasing-overlay/)
- [Buildkite Com Rest Api Overlay](https://apis.io/overlays/buildkite-com/buildkite-com-rest-api-overlay/)
- [Buildkite Com Rules Api Phrasing Overlay](https://apis.io/overlays/buildkite-com/buildkite-com-rules-api-phrasing-overlay/)
- [Buildkite Com Stacks Api Phrasing Overlay](https://apis.io/overlays/buildkite-com/buildkite-com-stacks-api-phrasing-overlay/)
- [Buildkite Com Teams Api Phrasing Overlay](https://apis.io/overlays/buildkite-com/buildkite-com-teams-api-phrasing-overlay/)
- [Buildkite Com User Api Phrasing Overlay](https://apis.io/overlays/buildkite-com/buildkite-com-user-api-phrasing-overlay/)

#### Governance rules (3)

Spectral rulesets for the provider's contracts.

- [Buildkite — jsonschema rules](https://apis.io/rules/buildkite-com/buildkite-com-jsonschema-spectral-rules/)
- [Buildkite API Rules](https://apis.io/rules/buildkite-com/buildkite-com-rules/)
- [Buildkite — buildkite rules](https://apis.io/rules/buildkite-com/buildkite-rules/)

#### Security (3)

Authentication, trust centre, and vulnerability disclosure.

- [Buildkite Com Authentication](https://apis.io/security/buildkite-com/buildkite-com-authentication/)
- [Buildkite Com Domain Security](https://apis.io/security/buildkite-com/buildkite-com-domain-security/)
- [Buildkite Com Trust Center](https://apis.io/security/buildkite-com/buildkite-com-trust-center/)

#### OAuth scopes (1)

The permissions the API asks for.

- [Buildkite Com Scopes](https://apis.io/scopes/buildkite-com/buildkite-com-scopes/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [Buildkite Com Plans Pricing](https://apis.io/plans/buildkite-com/buildkite-com-plans-pricing/)

#### Rate limits (1)

Published request limits.

- [Buildkite Com Rate Limits](https://apis.io/rate-limits/buildkite-com/buildkite-com-rate-limits/)

#### FinOps (1)

What the API costs to run, by operation.

- [Buildkite Com Finops](https://apis.io/finops/buildkite-com/buildkite-com-finops/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://www.buildkite.com/)
- [Documentation](https://buildkite.com/docs)
- [Getting started](https://buildkite.com/docs/tutorials/getting-started)
- [Pricing](https://buildkite.com/pricing)
- [Support](https://buildkite.com/support)
- [Changelog](https://buildkite.com/changelog)
- [Blog](https://buildkite.com/blog)
- [Compliance](https://trust.buildkite.com/)
- [Trust centre](https://buildkite.com/security)
- [Terms of service](https://buildkite.com/legal/terms-of-service)
- [Privacy policy](https://buildkite.com/legal/privacy-policy)
- [GitHub](https://github.com/buildkite)
- [Status](https://buildkitestatus.com)

## API Evangelist rating

**Kin Score 66.5** — exemplar · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 68.3 |
| Contract quality | 66.0 |
| Contract governance | 31.8 |
| Operational transparency | 63.2 |
| Developer ergonomics | 72.6 |
| Access clarity | 68.4 |

**Agent readiness 50.6** — agent-ready (gated down from agent-native)

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | documented (partial credit) |
| MCP Server | verified |
| Auth Clarity | served (partial credit) |
| Idempotency | — |
| Error Semantics | derived (partial credit) |
| OpenAPI Examples | — |
| Rate Limit Signal | documented (partial credit) |
| Event Surface Described | yes |
| Agent Skills | — |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | served (partial credit) |
| Protected Resource Metadata | verified |
| Dynamic Client Registration | yes |
| Agentic Commerce | — |
| Pagination Ratio | — |
| Operation Distinctiveness | distinct |

**Regulatory alignment 39.2** — Horizontal (data, software, accessibility, platform)

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/buildkite-com/](https://apis.io/providers/buildkite-com/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Buildkite: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/buildkite-com/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
