---
title: "Know when the Buildkite CLI is done or needs you, without watching its tab"
url: "https://buildkite.com/resources/changelog/425-know-when-the-buildkite-cli-is-done-or-needs-you-without-watching-its-tab/"
date: "2026-10-16"
author: "Mark Wolfe"
feed_url: "https://buildkite.com/changelog.atom"
---
You can now see when bk preflight or bk build watch finishes or needs you, without switching back to its tab. From Buildkite CLI v3.64.0 , bk tells your terminal what it's doing, so a terminal that supports it can show you while you work somewhere else. bk reports its status using OSC 7501 , a draft protocol that lets programs tell the terminal whether they're working, waiting on the user, done, or failed.
