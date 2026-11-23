---
source: x
author: @kunchenguid
date: 2026-11-21
url: https://x.com/kunchenguid/status/2123985561551778151
pile: reread
topic: AI Agents & Dev Tools
tags: [bookmark, reread]
---

# Batching branches into one PR to cut CI load

Kun Chen (@kunchenguid) says his PR count fell from about 200 a day to around 30, while he is shipping more than ever, by batching multiple finished branches into a single PR. Each change still gets its own branch. A branch that is done gets a lightweight CI check (mostly build and lint). Passing branches queue into a batch, and a batch becomes one PR that runs the heavier CI. While that PR is open, new branches wait for the next batch, so he has at most one open PR per repo at a time. If CI fails, he fix-forwards by adding a new branch to the same batch, leaving older branches immutable and avoiding rebases.

He argues this beats a repo-level merge queue: at agent speed a merge queue can hold hundreds of PRs, break often, and force re-selection and waiting. Batching is per user, so contributors don't block each other, and people in the same repo can mix strategies (one PR per branch, or this batch).

**Why it matters:** A concrete answer to the CI and review bottleneck of high-volume agent PRs — relevant if you're generating a lot of branches and paying for redundant checks.

**What to try:** In one busy repo, try a per-user batch: light checks per branch, one heavier PR at a time, and fix-forward with a new branch instead of rebasing when CI fails.

[Open post](https://x.com/kunchenguid/status/2123985561551778151)
