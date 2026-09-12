---
title: "Job acquisition tokens for ephemeral agents"
url: "https://buildkite.com/resources/changelog/401-job-acquisition-tokens-for-ephemeral-agents/"
date: "2026-08-31"
author: "Steven Webb"
feed_url: "https://buildkite.com/changelog.atom"
---
Stack-managed ephemeral agents can now start with a credential for one job. The controller keeps its cluster agent token and issues a short-lived job acquisition token (JAT) after reserving work. The workload uses that JAT to register an agent and acquire only the named job.
