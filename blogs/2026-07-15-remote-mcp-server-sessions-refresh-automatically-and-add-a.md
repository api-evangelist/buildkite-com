---
title: "Remote MCP Server sessions refresh automatically and add a redirect confirmation step"
url: "https://buildkite.com/resources/changelog/374-remote-mcp-server-sessions-refresh-automatically-and-add-a-redirect-confirmation-step/"
date: "2026-07-15"
author: "Mark Wolfe"
feed_url: "https://buildkite.com/changelog.atom"
---
The Remote MCP Server 's OAuth flow has had several reliability and security improvements, changing how MCP client sessions stay authenticated. Sessions refresh instead of expiring Previously, a session was tied to a fixed 7-day refresh token, after which an MCP client had to go through the full interactive authorization flow again. Sessions are now refreshed continuously in the background: access tokens are short-lived (1 hour) and refresh tokens roll forward for up to 30 days of continued use, so an actively used agent no longer hits a hard weekly re-authentication wall.
