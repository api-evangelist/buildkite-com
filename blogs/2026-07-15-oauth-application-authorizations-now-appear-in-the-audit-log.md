---
title: "OAuth application authorizations now appear in the audit log"
url: "https://buildkite.com/resources/changelog/373-oauth-application-authorizations-now-appear-in-the-audit-log/"
date: "2026-07-15"
author: "Ben McNicholl"
feed_url: "https://buildkite.com/changelog.atom"
---
Organization administrators can now see when a user authorizes an OAuth application to access their organization in the Buildkite audit log . Each OAUTH_APPLICATION_AUTHORIZED event identifies the user, OAuth application, organization, granted scopes, request IP address, and User Agent. This provides a clearer record of when tools using OAuth—such as the Buildkite CLI and Remote MCP Server—are granted access.
