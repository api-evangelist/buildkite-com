---
title: "Read-only GitHub Actions, Variables, and Environments permissions"
url: "https://buildkite.com/resources/changelog/404-read-only-github-actions-variables-and-environments-permissions/"
date: "2026-09-02"
author: "Lachlan Donald"
feed_url: "https://buildkite.com/changelog.atom"
---
{% raw %}
To improve GitHub Actions migration support , the Buildkite GitHub App now requests read-only access to Actions , Variables , and Environments . These permissions let Buildkite inspect configuration that affects how workflows and deployments run—including configuration variables referenced through ${{ vars.* }} , secret names (not secret values), deployment protection rules, and deployment branch policies—so migrated pipelines can preserve existing behavior and safeguards. All three permissions are read-only; Buildkite will not modify Actions workflows, variables, or environments.
{% endraw %}
