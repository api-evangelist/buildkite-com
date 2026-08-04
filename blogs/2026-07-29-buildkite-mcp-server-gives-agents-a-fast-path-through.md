---
title: "Buildkite MCP Server gives agents a fast path through failed builds"
url: "https://buildkite.com/resources/changelog/381-buildkite-mcp-server-gives-agents-a-fast-path-through-failed-builds/"
date: "2026-07-29"
author: "Ben McNicholl"
feed_url: "https://buildkite.com/changelog.atom"
---
Debugging a failed build shouldn't start with a scavenger hunt. The Buildkite MCP Server now includes get_build_failure_summary , a new tool designed around Anthropic's best practices for writing tools for agents . It turns a common multi-step workflow into one purpose-built call, taking an agent from “the build failed” to a likely cause.
