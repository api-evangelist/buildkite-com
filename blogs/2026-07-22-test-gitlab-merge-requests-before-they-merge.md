---
title: "Test GitLab merge requests before they merge"
url: "https://buildkite.com/resources/changelog/378-test-gitlab-merge-requests-before-they-merge/"
date: "2026-07-22"
author: "Hannah Thompson"
feed_url: "https://buildkite.com/changelog.atom"
---
Teams using GitLab.com or GitLab Self-Managed can now build merge requests and test proposed merges against their target branches with merged-results builds. Merge request builds test the source branch, while merged-results builds test the proposed merge, helping catch integration failures before merging. Set up merge request builds In your pipeline's GitLab settings: Enable Build merge requests to build a merge request when it opens or receives new commits.
