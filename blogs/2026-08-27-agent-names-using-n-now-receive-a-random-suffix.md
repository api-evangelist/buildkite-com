---
title: "Agent names using `%n` now receive a random suffix"
url: "https://buildkite.com/resources/changelog/400-agent-names-using-percentn-now-receive-a-random-suffix/"
date: "2026-08-27"
author: "Benno Moskovitz"
feed_url: "https://buildkite.com/changelog.atom"
---
Agent names containing %n now receive a random six-character alphanumeric suffix instead of the next available number. For example, cool-agent-%n , which previously produced a name such as cool-agent-123 , now produces a name such as cool-agent-aB3dE6 . We deprecated %n in 2022 because allocating sequential agent names becomes increasingly expensive as organizations scale.
