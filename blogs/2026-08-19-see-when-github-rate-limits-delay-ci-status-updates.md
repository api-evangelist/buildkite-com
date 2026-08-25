---
title: "See when GitHub rate limits delay CI status updates"
url: "https://buildkite.com/resources/changelog/393-see-when-github-rate-limits-delay-ci-status-updates/"
date: "2026-08-19"
author: "Owen Mehegan"
feed_url: "https://buildkite.com/changelog.atom"
---
When a build has finished but its status hasn't appeared on a pull request, it can be difficult to tell whether CI is still processing or GitHub is temporarily unable to accept the update. Buildkite now surfaces GitHub API rate-limit exhaustion directly in the UI, giving you clear visibility into what's delaying status updates and when normal delivery should resume. What we're doing We've added an organization-wide banner that appears when the API quota for your GitHub App installation is exhausted.
