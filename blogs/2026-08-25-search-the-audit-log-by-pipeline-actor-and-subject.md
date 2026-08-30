---
title: "Search the audit log by pipeline, actor, and subject"
url: "https://buildkite.com/resources/changelog/397-search-the-audit-log-by-pipeline-actor-and-subject/"
date: "2026-08-25"
author: "Pete Tomasik"
feed_url: "https://buildkite.com/changelog.atom"
---
Buildkite's audit log search was previously limited to type: , so answering "what happened to this pipeline?" or "what did this person change?" meant paging through everything else that happened in the last 90 days. We've added three more terms to help you find exactly what you're looking for. pipeline: returns the events a pipeline is the subject of, by slug or UUID (for example, pipeline:my-app ).
