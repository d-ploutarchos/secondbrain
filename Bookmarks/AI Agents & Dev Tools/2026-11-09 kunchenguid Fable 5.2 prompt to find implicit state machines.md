---
source: x
author: @kunchenguid
date: 2026-11-09
url: https://x.com/kunchenguid/status/2119924895060795492
pile: tool
topic: AI Agents & Dev Tools
tags: [bookmark, tool]
---

# Fable 5.2 prompt to find implicit state machines

Kun Chen shares a prompt for feeling Fable 5.2's strength: "audit and find implicit state machines in this <codebase/directory/module> that would drive concrete improvements if made explicit. explain before/after of each one and discuss with me in lavish-axi. fewer words, big visuals." [lavish-axi](https://github.com/kunchenguid/lavish-axi) is optional and makes the findings easier to judge. The attached example from the firstmate repo: "Away" stored in two places that can disagree (posture record vs supervisor flag), so two of three readers think you are not away; the fix is one canonical answer. Quotes Steve Ruiz: "find all of the implicit state machines in my app." He says 5.2 is good at spotting real problems, ignoring noise, and explaining them intuitively.

**Why it matters:** A sharp, reusable audit prompt for the new Fable 5.2, plus a visualization helper.

**What to try:** Run the prompt on a module you suspect has split or implicit state; add lavish-axi if you want the before/after diagrams.

[Open post](https://x.com/kunchenguid/status/2119924895060795492)
