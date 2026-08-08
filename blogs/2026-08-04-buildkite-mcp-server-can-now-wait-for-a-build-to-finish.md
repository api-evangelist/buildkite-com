---
title: "Buildkite MCP Server can now wait for a build to finish"
url: "https://buildkite.com/resources/changelog/385-buildkite-mcp-server-can-now-wait-for-a-build-to-finish/"
date: "2026-08-04"
author: "Mark Wolfe"
feed_url: "https://buildkite.com/changelog.atom"
---
Agents no longer need to hand-roll a polling loop over get_build to find out how a build went. The Buildkite MCP Server now includes wait_for_build , a tool that waits for a build to reach a terminal state and reports the outcome. Each call waits up to 45 seconds.
