---
title: "Retry jobs with narrower API token permissions"
url: "https://buildkite.com/resources/changelog/421-retry-jobs-with-narrower-api-token-permissions/"
date: "2026-10-13"
author: "Ben McNicholl"
feed_url: "https://buildkite.com/changelog.atom"
---
Retry automation no longer needs the broader write_builds REST API scope. The new retry_builds scope allows a token to retry failed jobs in existing builds or individual eligible jobs, without granting access to the create-build or rebuild endpoints. When creating or editing an API access token, select Build Retries ( retry_builds ).
