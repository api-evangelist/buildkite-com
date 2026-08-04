---
title: "Buildkite MCP Server adds job tools and smarter artifact and log handling"
url: "https://buildkite.com/resources/changelog/371-buildkite-mcp-server-adds-job-tools-and-smarter-artifact-and-log-handling/"
date: "2026-07-13"
author: "Mark Wolfe"
feed_url: "https://buildkite.com/changelog.atom"
---
The Buildkite MCP Server has new tools for working with jobs, smarter artifact and log handling, and more scalable pagination for large builds and test runs. Dedicated tools for inspecting jobs Agents can now look up job details directly with list_jobs and get_job , filter by state (for example, only failed jobs), page through large builds efficiently, and pull full agent details only when needed. This makes it much faster for an agent to zero in on "why did this build fail?" without wading through unrelated build metadata.
