---
source: x
author: @mattpocockuk
date: 2026-11-20
url: https://x.com/mattpocockuk/status/2123798388227403983
pile: tool
topic: AI Agents & Dev Tools
tags: [bookmark, tool]
---

# Prompt to audit and delete code comments

Matt Pocock (@mattpocockuk) posts a long "prompt of the day" for cleaning comments, and says he is sold: comments considered harmful. The prompt asks an agent to review every comment in a codebase (or a section) and classify each as tautology (repeats what the code already shows), excuse (covers for a hack that then spreads), stale (refers to code that is gone), or decision record (a non-obvious choice). Then: delete tautologies and stale comments; delete excuses and file an issue to fix the hack; move decision records into an ADR. Afterwards, add a lint rule banning comments in that area, ratchet so this PR doesn't have to delete everything, create a `/delete-comment` skill to repeat later, and estimate how many lines you'll shed.

**Why it matters:** A copyable comment-cleanup prompt that also leaves a lint ratchet and a skill, in the same "comments waste tokens" vein as Georgios's swarm-ready checklist.

**What to try:** Run the prompt on one section of a repo you own, keep the ADRs, and add the lint ratchet plus a `/delete-comment` skill if the first pass is useful.

[Open post](https://x.com/mattpocockuk/status/2123798388227403983)
