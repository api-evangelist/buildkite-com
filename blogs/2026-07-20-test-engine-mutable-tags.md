---
title: "Test Engine mutable tags"
url: "https://buildkite.com/resources/changelog/376-test-engine-mutable-tags/"
date: "2026-07-20"
author: "Malcolm Locke"
feed_url: "https://buildkite.com/changelog.atom"
---
Test execution results uploaded to Test Engine are immutable, and so cannot be updated after initial upload. To allow metadata to be attached to execution records after upload we have introduced mutable tags . Additional tags can be attached to executions in bulk via the execution tags API endpoint .
