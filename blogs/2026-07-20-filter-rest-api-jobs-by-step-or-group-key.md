---
title: "Filter REST API jobs by step or group key"
url: "https://buildkite.com/resources/changelog/375-filter-rest-api-jobs-by-step-or-group-key/"
date: "2026-07-20"
author: "Buildkite"
feed_url: "https://buildkite.com/changelog.atom"
---
The REST API's List Jobs endpoint now accepts optional step_key and group_key filters. Use step_key to return the jobs for a specific step, including every job in a parallel step. Use group_key to return all jobs in a step group.
