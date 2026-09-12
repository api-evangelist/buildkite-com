---
title: "SSH into Linux hosted jobs from the Buildkite CLI"
url: "https://buildkite.com/resources/changelog/402-ssh-into-linux-hosted-jobs-from-the-buildkite-cli/"
date: "2026-09-01"
author: "Jamie Monserrate"
feed_url: "https://buildkite.com/changelog.atom"
---
You can now connect to running Linux hosted jobs over SSH from your terminal using the Buildkite CLI . This extends the existing bk job ssh command for macOS hosted jobs to Linux hosted agents. Install Buildkite CLI version 3.55.1 or later, then run: bk job ssh The command opens an interactive shell and forwards terminal size and resize events.
