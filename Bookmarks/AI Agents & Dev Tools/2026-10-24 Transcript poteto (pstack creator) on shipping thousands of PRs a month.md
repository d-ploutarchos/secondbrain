---
source: x
author: @shydev69
date: 2026-10-24
url: https://x.com/shydev69/status/2113904540080881716
pile: reread
topic: AI Agents & Dev Tools
tags: [bookmark, reread]
---

# Transcript: poteto (pstack creator) on shipping thousands of PRs a month

Reply linking a GitHub gist with the full transcript of a live podcast where Matt Pocock interviews poteto (ex-React team at Meta, now at Cursor / SpaceX AI, creator of the pstack skills) about shipping 2,500 PRs in a month. Key ideas: a trust ladder where you hand agents more as they earn it; a 'Michelin kitchen' framing instead of 'software factory' (scale without giving up craft); skills as thin wrappers that push deterministic steps into scripts/CLIs so the agent only spends judgment where it's needed; strict codebase conventions and lint rules (one way to do each thing, a directory per feature, no god files) so agents can't easily write bad code; review by sampling and fixing the environment when several agents repeat a mistake, rather than reading every PR; and letting agents merge their own work only where it can be truly verified.

**Why it matters:** The clearest long-form explanation of how a high-output agent setup actually works, from someone running one; worth rereading when shaping your own agent workflows.

**What to try:** Pick one recurring agent mistake in your repos and fix it in the environment (a lint rule, convention, or script) instead of in the prompt; move one deterministic step of a skill into a script.

Transcript gist: https://gist.github.com/ayush-that/809328c80b267ffa1d23349f4bfebbac

[Open post](https://x.com/shydev69/status/2113904540080881716)
