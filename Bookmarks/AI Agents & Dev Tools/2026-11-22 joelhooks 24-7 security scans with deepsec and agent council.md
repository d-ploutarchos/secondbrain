---
source: x
author: @joelhooks
date: 2026-11-22
url: https://x.com/joelhooks/status/2124369230154064301
pile: tool
topic: AI Agents & Dev Tools
tags: [bookmark, tool]
---

# 24/7 security scans with deepsec and an agent council

Joel Hooks (@joelhooks) has been running around-the-clock security scans for a week with a local model (glm-flash) on Vercel Labs' [deepsec](https://github.com/vercel-labs/deepsec), a coding-agent harness for finding vulnerabilities in your codebase. He says it is "v good" and is surfacing issues constantly — hundreds of them. Findings get passed to an agent council (Theo's tstack skill) to fix.

**Why it matters:** A working loop for continuous, local-model security scanning plus an automated fix council, using a concrete open-source harness rather than a one-off prompt.

**What to try:** Point deepsec at a repo you own, start with a local or cheap model, and only then wire high-confidence findings into a fix council. Treat it as defensive testing of your own code.

[Open post](https://x.com/joelhooks/status/2124369230154064301)
