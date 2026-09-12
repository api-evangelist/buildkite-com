---
title: "Job logs are limited to 1 GiB"
url: "https://buildkite.com/resources/changelog/405-job-logs-are-limited-to-1-gib/"
date: "2026-09-03"
author: "Juanito Fatas"
feed_url: "https://buildkite.com/changelog.atom"
---
Job logs are now limited to 1 GiB (1,024 MiB) by default. You can check your organization’s current log size limit on the Quotas page . When a job log exceeds the limit, Buildkite cancels the job and adds a Log Size Limit Exceeded event to the timeline.
