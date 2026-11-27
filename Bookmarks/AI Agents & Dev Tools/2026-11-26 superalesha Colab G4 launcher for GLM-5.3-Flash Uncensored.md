---
source: x
author: @superalesha
date: 2026-11-26
url: https://x.com/superalesha/status/2126011712692224264
pile: tool
topic: AI Agents & Dev Tools
tags: [bookmark, tool]
---

# Colab G4 launcher for GLM-5.3-Flash Uncensored

Alexey Fateev (@superalesha) points out that a Gemini or Google AI subscription already includes Colab compute units, which can run a G4 instance (96 GB RTX PRO 6000 Blackwell, 176 GB RAM) at 10.05 CU/hr -- cheaper than an H100, with more VRAM. He packed a launcher that starts GLM-5.3-Flash Uncensored (321B, abliterated EXL3 on Project Maya + DFlash2) in about 10 minutes and tunnels a local OpenAI /v1 and Anthropic /v1/messages API to 127.0.0.1:18100, with tool calls, thinking, vision, and no refusals. Default 2.51 bpw hits about 102 tok/s decode at 131K context; higher quantizations trade speed for quality. The script prints ready-to-paste snippets for Claude Code, Codex, or OpenCode, and ships with a stop script so idle units don't keep burning. Repo, scripts, and tuned Maya configs: https://github.com/alesha-pro/tools/tree/main/colab-g4-glm53

Hours of G4 time included: Pro ($20/mo) ~20 hours, Ultra 5x ($100) ~99 hours, Ultra 20x ($200) ~199 hours. In later replies he warned that once the post spread, G4 cards became hard to grab, and he polished the script with backoff retries and keep-alive pings so Google doesn't drop an idle session.

**Why it matters:** A concrete way to turn a Google AI subscription you may already pay for into a fast, uncensored local-feeling endpoint for a coding harness, without buying a 96 GB GPU.

**What to try:** If you have a Gemini or Google AI plan, run the launcher from the repo on a Colab G4, point Claude Code, Codex, or OpenCode at the local endpoint, and use the stop script when you're done so you don't burn compute units.

[Open post](https://x.com/superalesha/status/2126011712692224264)
