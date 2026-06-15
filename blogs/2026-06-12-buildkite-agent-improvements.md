---
title: "Buildkite Agent improvements"
url: "https://buildkite.com/resources/changelog/364-buildkite-agent-improvements/"
date: "2026-06-12"
author: "Buildkite"
feed_url: "https://buildkite.com:443/changelog.atom"
---
Checkout Skip checkout on any agent by setting BUILDKITE_SKIP_CHECKOUT=true — no plugin or workaround required. Previously this meant clearing BUILDKITE_REPO , using a checkout plugin, or (in the Agent Stack for Kubernetes) setting checkout: skip: true . Skip fetching commits you already have with --git-skip-fetch-existing-commits , which skips the git fetch step during checkout when the target commit already exists locally.
