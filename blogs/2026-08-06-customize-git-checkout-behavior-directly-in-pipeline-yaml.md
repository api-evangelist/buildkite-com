---
title: "Customize Git checkout behavior directly in pipeline YAML"
url: "https://buildkite.com/resources/changelog/389-customize-git-checkout-behavior-directly-in-pipeline-yaml/"
date: "2026-08-06"
author: "Owen Mehegan"
feed_url: "https://buildkite.com/changelog.atom"
---
You can now configure how the Buildkite agent checks out your source code using a new checkout block in your pipeline YAML. Skip checkout entirely, perform shallow clones, set custom Git flags, and more - all from within your pipeline definition. For example: checkout: submodules: false steps: - label: "Fast build" command: "make build" checkout: depth: 50 sparse: paths: - src/ - .buildkite/ - label: "Full integration tests" command: "make integration" checkout: submodules: true The checkout block can be set at both the pipeline level (as a default for all steps) and the step level (to overrid
