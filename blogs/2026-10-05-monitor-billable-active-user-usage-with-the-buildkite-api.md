---
title: "Monitor billable active-user usage with the Buildkite API"
url: "https://buildkite.com/resources/changelog/419-monitor-billable-active-user-usage-with-the-buildkite-api/"
date: "2026-10-05"
author: "Buildkite"
feed_url: "https://buildkite.com/changelog.atom"
---
You can now monitor your organization's billable active-user usage programmatically and compare it with your contracted allowance. Send the count to observability tools such as Datadog to track usage over time, or include it in internal license, billing, and compliance reporting. The Average monthly active users figure shown on the Organization Usage page is available through both Buildkite APIs: REST: GET /v2/organizations/{org}/usage returns { "active_users_count": } and requires the read_organizations scope.
