---
title: "Diagnose infrastructure-related job failures through the REST API"
url: "https://buildkite.com/resources/changelog/369-diagnose-infrastructure-related-job-failures-through-the-rest-api/"
date: "2026-06-29"
author: "Sarah Jackson"
feed_url: "https://buildkite.com/changelog.atom"
---
Buildkite's REST API now exposes more of the job and runner context that agents, CLI tools, and MCP clients need to tell infrastructure failures apart from code failures. The REST job object now includes signal and signal_reason . When signal_reason is present, it explains why the Buildkite Agent terminated the job, such as agent_stop or process_run_error .
