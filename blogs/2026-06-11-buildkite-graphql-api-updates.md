---
title: "Buildkite GraphQL API updates"
url: "https://buildkite.com/resources/changelog/361-buildkite-graphql-api-updates/"
date: "2026-06-11"
author: "Buildkite"
feed_url: "https://buildkite.com:443/changelog.atom"
---
The metaData field on builds and jobs now supports up to 1 MB of total data, up from the previous 64 KB limit. If you've been hitting size constraints when attaching metadata to builds, this gives you significantly more room. Job annotations are now accessible through the GraphQL API.
