---
title: "Send job logs to your OpenTelemetry collector"
url: "https://buildkite.com/resources/changelog/386-send-job-logs-to-your-opentelemetry-collector/"
date: "2026-08-05"
author: "Ming Guo"
feed_url: "https://buildkite.com/changelog.atom"
---
Buildkite Agent v3.135.0 can now send job logs to your OpenTelemetry collector. This brings CI output into the same observability backend as your application and infrastructure telemetry, making it easier to investigate slow or failing jobs without switching between tools. When OpenTelemetry tracing is also enabled, each record is correlated with the job, phase, or hook span that produced it.
