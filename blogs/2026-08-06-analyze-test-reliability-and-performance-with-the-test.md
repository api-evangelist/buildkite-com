---
title: "Analyze test reliability and performance with the Test Engine API"
url: "https://buildkite.com/resources/changelog/390-analyze-test-reliability-and-performance-with-the-test-engine-api/"
date: "2026-08-06"
author: "Meghan Kradolfer"
feed_url: "https://buildkite.com/changelog.atom"
---
The Test Engine List tests API now returns aggregated reliability, duration, and execution metrics for each test. You can use these metrics to identify your flakiest or slowest tests. The endpoint also supports: Filtering by branch, labels, owners, state, and tags Selecting a relative period or an explicit timestamp range Sorting by reliability or average, total, minimum, or maximum duration Paginating results using the response's Link header To use the updated response, include this header with your request: Buildkite-Version: 2026-08-01 The header is the only opt-in required.
