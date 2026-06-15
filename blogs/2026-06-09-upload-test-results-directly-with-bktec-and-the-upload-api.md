---
title: "Upload test results directly with bktec and the Upload API"
url: "https://buildkite.com/resources/changelog/358-upload-test-results-directly-with-bktec-and-the-upload-api/"
date: "2026-06-09"
author: "Naufan P. Rizal"
feed_url: "https://buildkite.com:443/changelog.atom"
---
You can now upload test results directly to Test Engine, either through bktec v2.7.0's new upload option, or by pushing raw output yourself via the Upload API. Test collectors are still supported, but they're no longer a hard dependency. bktec v2.7.0 - direct result uploads bktec v2.7.0 adds a new BUILDKITE_TEST_ENGINE_UPLOAD_RESULTS option and --upload-results flag to upload your test runner's raw output straight to the Upload API.
