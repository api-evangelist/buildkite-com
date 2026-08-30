---
title: "Additional GitHub App permissions for GitHub Actions workflows"
url: "https://buildkite.com/resources/changelog/396-additional-github-app-permissions-for-github-actions-workflows/"
date: "2026-08-25"
author: "Jordan Carter"
feed_url: "https://buildkite.com/changelog.atom"
---
To expand GitHub Actions workflow support , the Buildkite GitHub App now requests read and write access to Issues , Packages , Attestations , and Artifact metadata . These permissions allow compatible workflows to respond to issue activity, publish GitHub Packages, and create artifact attestations and metadata. Existing installations will be prompted in GitHub to approve them.
