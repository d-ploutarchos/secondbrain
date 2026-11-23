---
source: x
author: @pontusab
date: 2026-11-20
url: https://x.com/pontusab/status/2123750671795261748
pile: tool
topic: AI Agents & Dev Tools
tags: [bookmark, tool]
---

# Full CI pipeline now sub 1 min with bun

Pontus Abrahamsson (@pontusab, building Glass at @tryramp) got his full CI pipeline under one minute. The recipe: Vitest → `bun test`, tsc → `bun check`, oxlint → `bun lint`, oxfmt → `bun fmt`; shards filled by recorded test time; PRs run only the tests the diff can reach; the backend builds the app once per process; lint, typecheck, build, and tests all run in parallel. He says that saves 200+ hours of waiting every week.

**Why it matters:** A specific, copyable CI speed recipe — especially relevant if agent-driven PRs are spending a lot of time in checks.

**What to try:** On one JS/TS repo, switch tests, typecheck, lint, and format to the bun tools, run those jobs in parallel, and restrict PR tests to what the diff can reach.

[Open post](https://x.com/pontusab/status/2123750671795261748)
