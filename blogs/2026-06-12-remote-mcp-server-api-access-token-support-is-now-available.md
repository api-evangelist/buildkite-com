---
title: "Remote MCP Server API access token support is now available (Preview)"
url: "https://buildkite.com/resources/changelog/363-remote-mcp-server-api-access-token-support-is-now-available-preview/"
date: "2026-06-12"
author: "Mark Wolfe"
feed_url: "https://buildkite.com:443/changelog.atom"
---
A preview of Buildkite API access token authentication for the Buildkite Remote MCP Server is now available through a dedicated endpoint: https://mcp.buildkite.com/direct . Use this endpoint for headless or background agents that already have a Buildkite API access token and do not need the interactive OAuth flow. This helps avoid contention around shared OAuth tokens when multiple background agents are running at once.
