---
title: "Buildkite MCP Server trims job list payloads and adds annotation summaries"
url: "https://buildkite.com/resources/changelog/377-buildkite-mcp-server-trims-job-list-payloads-and-adds-annotation-summaries/"
date: "2026-07-21"
author: "Mark Wolfe"
feed_url: "https://buildkite.com/changelog.atom"
---
The Buildkite MCP Server now returns leaner job data by default and surfaces build annotations without extra round trips. Smaller, more targeted job listings list_jobs now returns compact, actionable summaries by default, reducing token usage while keeping job IDs and failure diagnostics. Use detail_level: "detailed" for execution metadata, or detail_level: "full" for the previous, more verbose response.
