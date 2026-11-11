---
source: x
author: @bebuu_ai
date: 2026-11-10
url: https://x.com/bebuu_ai/status/2120080226801820156
pile: tool
topic: AI Agents & Dev Tools
tags: [bookmark, tool]
---

# Fable 5.2 ownership prompt so it treats the repo as yours

bebu notes a finding from Anthropic’s Claude Fable 5.2 prompting guide: if you give Fable 5.2 a coding task without saying who owns the repo, it assumes it is a guest in someone else’s codebase. It then plays it safe — bolting new functions onto the existing structure, leaving duplicate code alone, and only mentioning nearby bugs instead of fixing them. Adding this sentence to the system prompt or CLAUDE.md changes that: “This codebase is yours: what it's for and how it's built are your call, and you'll keep building on it.” In Anthropic’s internal tests, that one line made Fable 5.2 proactively merge duplicate code and clean up related bugs in about 50% of runs, versus under 10% without it.

**Why it matters:** A one-line prompt change that shifts Fable 5.2 from cautious guest to owner, which matches how you actually want agents to work in your own repos.

**What to try:** Add that ownership sentence to CLAUDE.md (or the equivalent system prompt) in a repo you own and see whether cleanup and deduping become more proactive.

[Open post](https://x.com/bebuu_ai/status/2120080226801820156)
