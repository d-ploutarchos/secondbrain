---
source: x
author: @gakonst
date: 2026-11-20
url: https://x.com/gakonst/status/2123839118409109853
pile: reread
topic: AI Agents & Dev Tools
tags: [bookmark, reread]
---

# Effective Swarm Riding for Engineers

Georgios Konstantopoulos (@gakonst, Paradigm GP/CTO and eng lead at Tempo) published [Effective Swarm Riding for Engineers](https://www.paradigm.xyz/writing/swarms), arguing that swarms only became practical with models like Opus 5.5, and that using them well takes the right attitude, infrastructure, and short "incantations." He applies the same ideas in [Nanocode](https://github.com/nanocodexyz/nanocode), a swarm harness that runs locally or in your own cloud, uses code mode, and can sit on Claude, Codex, or Antigravity backends.

His principles: be unreasonably ambitious (rewrite the slow or unsafe parts of your stack — even a database or crypto — the way they rebuilt Tempo in more than five languages in days). Use cloud agents so work runs 24/7, via Nanocode, Pi Durable, Fx, a well-known product, or a bootleg devbox. Prefer short, dense prompts over long specs: ask for "10x faster" not "optimize X"; "differentially test this and close all gaps" not "fix all bugs"; "using TigerStyle reimplement in <lang>"; and persistence prompts like "I am stepping away for 8hrs, believe in yourself." He also likes "superpowered find-and-replace" prompts (implicit state machines into the type system, shared state into lock-free tokio actors, sequential async into `tokio::join`, add otel and measure bottlenecks). Do the simple thing: frontier models, a well-set-up codebase, and get out of the way — he says not to build plans, orchestration, memory, compaction, skills, or cross-review, because each model cycle wipes last cycle's customizations.

To make a codebase swarm-ready, he would: strip comments (they waste tokens and confuse agents); delete `.skills` and `docs/`; remove agent-written unit tests and ban them in AGENTS.md, replacing them with Deterministic Simulation Tests; rewrite dependencies / use TigerStyle against supply-chain risk; monorepo everything; and, controversially, push to master and treat the agent thread as the new PR and CI, with testing running on the same infra as the agents. Interaction should also change: an inbox that feeds one decision at a time (Superhuman-like), a loss-curve UI for performance work, or an infinite canvas for parallel ideas — not the default sidebar-plus-thread. He spends most of his time optimizing the environment, not the agent, and is most interested right now in automated program verification and testing.

**Why it matters:** A full, current operating manual for swarm-scale work from someone actually running it, including prompt patterns and a deliberately provocative codebase checklist. It sits next to the swarm-rider notes you've already filed.

**What to try:** Read the essay, then on a toy project try the dense prompts (especially "10x faster," differential testing, and an overnight "believe in yourself" run) and one or two swarm-ready changes that aren't the controversial "delete CI" step — for example stripping tautological comments or adding deterministic simulation tests. If you want his harness, try Nanocode.

[Open post](https://x.com/gakonst/status/2123839118409109853)
