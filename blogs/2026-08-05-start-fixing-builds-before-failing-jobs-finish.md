---
title: "Start fixing builds before failing jobs finish"
url: "https://buildkite.com/resources/changelog/388-start-fixing-builds-before-failing-jobs-finish/"
date: "2026-08-05"
author: "Chris Barrell"
feed_url: "https://buildkite.com/changelog.atom"
---
A long-running job can know it will exit non-zero before its command is complete. Until now, the build stayed running until that job finished, delaying notifications, investigation, and remediation. With promise job failure , the job can declare its expected exit status early.
