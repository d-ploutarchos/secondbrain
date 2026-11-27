---
source: x
author: @mvanhorn
date: 2026-11-26
url: https://x.com/mvanhorn/status/2125974014032323047
pile: tool
topic: AI Agents & Dev Tools
tags: [bookmark, tool]
---

# Tested 16 agent browser and computer-use tools

Matt Van Horn (@mvanhorn) tested 16 agent browser and computer-use tools on one Apple Silicon Mac so his T3 Code agents would stop handing work back to him. The article is "I Tested 16 Agent Browser and Computer-Use Tools. Here Is What I Switched To." (https://x.com/i/article/2125738584712056832).

The two browser winners are little-known on GitHub -- Ardia (~3k stars) and OpenCode browse (~1.1k) -- yet beat 54k-star agent-browser and 26k-star Stagehand on speed, RAM, and tokens. cua-driver (from @trycua, 32.9k stars) quietly powered five stacks in the test and won native Mac apps at 27 MB RAM with zero focus steal (597 ms on Messages, 129 ms on Electron).

What he switched to: Ardia + cua-driver. Fastest warm loads (396 ms), no Chrome 144 "Allow remote debugging?" popups, no debugging infobar, built-in prompt-injection fences, and full 1Password + Touch ID Passkeys. If you want to stay in Chrome: OpenCode browse + cua-driver, paired once over a Chrome extension so you can turn remote debugging off; 18 MB RAM and page snapshots 53x smaller than Stagehand and 5x smaller than agent-browser. Bonus: he wired the 1Password CLI to T3 Code over Touch ID so agents request secrets with a fingerprint tap. Boat was #1 for isolated cloud VMs (4 Ubuntu VMs in 1.9s median for $0.001). He also notes MIT / Rea work on turning desktop binaries into MCPs (FreeCAD 55x faster, 35x fewer tokens).

**Why it matters:** A same-machine scoreboard of the browser and computer-use stack, with clear winners and copy-paste setup prompts, instead of going by GitHub stars. Directly relevant if you want agents to drive a real logged-in browser and native Mac apps without stealing focus.

**What to try:** Read the article for the full scoreboard and setup prompts. If you want to switch, start with Ardia (https://ardia.dev) plus cua-driver (https://github.com/trycua/cua); if you want to stay in Chrome, use OpenCode browse (https://github.com/anomalyco/browse) plus cua-driver. Both have copy-paste setup prompts in the article.

[Open post](https://x.com/mvanhorn/status/2125974014032323047)
