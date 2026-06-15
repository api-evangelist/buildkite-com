---
title: "Dynamically update job timeouts with `buildkite-agent job update`"
url: "https://buildkite.com/resources/changelog/360-dynamically-update-job-timeouts-with-buildkite-agent-job-update/"
date: "2026-06-10"
author: "Matthew Borden"
feed_url: "https://buildkite.com:443/changelog.atom"
---
You can now update a job's timeout at runtime using the new buildkite-agent job update command. If a job discovers mid-run that it needs more (or less) time, it can adjust its own timeout without requiring a pipeline change. $ buildkite-agent job update timeout 20 This sets the job's timeout to 20 minutes.
