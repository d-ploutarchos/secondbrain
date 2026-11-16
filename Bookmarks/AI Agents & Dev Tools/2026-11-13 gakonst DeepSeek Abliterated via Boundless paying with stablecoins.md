---
source: x
author: @gakonst
date: 2026-11-13
url: https://x.com/gakonst/status/2121324288875835588
pile: tool
topic: AI Agents & Dev Tools
tags: [bookmark, tool]
---

# DeepSeek Abliterated via Boundless, paying with stablecoins

Georgios Konstantopoulos (@gakonst, Paradigm GP/CTO and eng lead at Tempo) says he is using DeepSeek Abliterated via Boundless, and paying with stablecoins, to hack Tempo. Boundless now serves an abliterated DeepSeek V4.1 Flash variant (fewer refusals, aimed at authorized security testing) and is the first inference provider on Tempo to accept MPP: an agent with a Tempo wallet can buy inference per request in USDC.e, OUSD, or MACH, with no Boundless account or API key. He also mentions `pmux`, a tmux hack tightly coupled with Tempo's internal cloud agents platform.

**Why it matters:** A live example of agents paying for their own inference on Tempo, including an abliterated model for security-style work — directly in the agent-payments lane you've been watching.

**What to try:** If you want an agent to buy its own tokens, follow Boundless's MPP setup (a Tempo wallet plus an MPP client such as `nanocode --gateway tempo`, endpoint `https://api.inference.boundless.network/mpp`). Treat the abliterated model as a defensive-testing tool, not a general-purpose one.

[Open post](https://x.com/gakonst/status/2121324288875835588)
