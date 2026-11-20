---
source: x
author: @wojkuli
date: 2026-11-19
url: https://x.com/wojkuli/status/2123400512594718847
pile: tool
topic: AI Agents & Dev Tools
tags: [bookmark, tool]
---
    10|
# Vercel Board plus Opus 5.5, boat, and e2e

Woj Kulikowski (@wojkuli) quotes Vercel's launch of Vercel Board, an experimental shared message board where people and agents coordinate tasks, exchange context, and work together across tools. He says combining Board with Opus 5.5, boat (@boatdotdev, cloud VM fleets for agents), and e2e (a software verification layer for agentic coding) is enough to "build anything with one prompt."

Vercel describes Board as a harness-agnostic primitive for agent fleets: channels and threads for tasks, permissions for humans and agents, two-way sync with tools like Slack and GitHub, and watchers that wake agents on new replies or label changes. Agents claim tasks, post updates, and complete work through a CLI or JavaScript SDK (`npx skills add vercel/board`). Vercel used it for internal security-agent swarms and rebuilt v0's software factory on it, which now merges over 50% of PRs. The announcement is at https://vercel.com/blog/introducing-vercel-board.

**Why it matters:** A concrete coordination layer for the swarm-style workflows you've been bookmarking, plus a suggested stack (model + Board + agent VMs + verification) rather than another vague "just use agents" claim.

**What to try:** Install the Board skill (`npx skills add vercel/board`) on a small project and have agents claim and complete tasks on a shared board. Optionally add boat for the agent VMs and e2e for verification, as Woj suggests.
    20|
[Open post](https://x.com/wojkuli/status/2123400512594718847)
