---
title: "Read-only API tokens no longer expose pipeline webhook URLs"
url: "https://buildkite.com/resources/changelog/368-read-only-api-tokens-no-longer-expose-pipeline-webhook-urls/"
date: "2026-06-22"
author: "Jonathan Ly"
feed_url: "https://buildkite.com/changelog.atom"
---
Read-only API access tokens no longer return a pipeline's webhook_url in REST and GraphQL responses. Previously, a read_only token created by someone with pipeline write access could still retrieve the webhook_url . Because that URL can be used to trigger builds, a token intended to be read-only could effectively grant write access.
