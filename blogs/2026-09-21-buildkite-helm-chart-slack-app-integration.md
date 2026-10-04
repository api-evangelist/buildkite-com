---
title: "Buildkite Helm chart: Slack App integration"
url: "https://buildkite.com/resources/changelog/410-buildkite-helm-chart-slack-app-integration/"
date: "2026-09-21"
author: "Buildkite"
feed_url: "https://buildkite.com/changelog.atom"
---
The Buildkite Agent Stack for Kubernetes Helm chart now includes built-in support for Slack App integration. You can configure Slack notifications directly in your Helm values without needing a separate sidecar or custom webhook setup. The chart handles token management and channel routing so your pipelines can post build status updates to Slack out of the box.
