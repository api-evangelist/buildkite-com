---
title: "Choose the organization for each Remote MCP Server connection"
url: "https://buildkite.com/resources/changelog/416-choose-the-organization-for-each-remote-mcp-server-connection/"
date: "2026-10-01"
author: "Samuel Cochran"
feed_url: "https://buildkite.com/changelog.atom"
---
If you belong to more than one Buildkite organization, you can now choose which one each Remote MCP Server connection uses. Add the organization's slug to the server URL: https://mcp.buildkite.com/mcp?organization=your-organization When your MCP client asks you to authorize, that organization is already selected. This also works with toolset and read-only URLs, such as https://mcp.buildkite.com/mcp/x/pipelines/readonly?organization=your-organization .
