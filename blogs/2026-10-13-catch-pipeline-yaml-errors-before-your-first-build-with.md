---
title: "Catch pipeline YAML errors before your first build with Buildkite MCP"
url: "https://buildkite.com/resources/changelog/423-catch-pipeline-yaml-errors-before-your-first-build-with-buildkite-mcp/"
date: "2026-10-13"
author: "Ben McNicholl"
feed_url: "https://buildkite.com/changelog.atom"
---
Your AI agent can now check the pipeline YAML it writes before you commit or upload it. The Buildkite MCP Server includes validate_pipeline , a read-only tool that checks YAML syntax and structure against Buildkite's pipeline schema, without uploading the pipeline or starting a build. Validation errors include paths and messages, giving your agent the information it needs to correct invalid step definitions and other schema errors.
