---
source: x
author: @gregisenberg
date: 2026-11-03
url: https://x.com/gregisenberg/status/2117734977312047537
pile: tool
topic: AI Agents & Dev Tools
tags: [bookmark, tool]
---

# Greg Isenberg's full agent stack for running a company

Greg Isenberg says he now talks to his agents more than his 50+ human teammates, and lays out the whole stack. Ideas start as a voice note to GrokBot, get interrogated with mattpocock/skills /grill-me, and land in Linear as specs; Exa, Firecrawl and Apify gather competitor sites and user reviews. Design runs in Claude Code with the Paper MCP (four versions of every screen, then merge the best parts). Builds run through pingdotgg/t3code and stablyai/orca (parallel agents in separate git worktrees), with graphify, headroom and LSP plugins; GitHub MCP opens PRs and Vercel makes previews. Lightpanda headless browsers test flows with different user personas, Sentry MCP errors become fix PRs, and a PostHog MCP job checks yesterday's funnel at 7am. Agents get their own computers (Orgo), inboxes (AgentMail) and phones (agentphone), plus git-backed markdown memory. Tricks: one agent per platform, a cheap model for triage, an LLM judge scoring every output, a 5-line nightly log per agent, and turning every agent mistake into a new skill.

**Why it matters:** It's a concrete, current map of tools for an agent-run company, and much of it (GrokBot, PostHog, Vercel, AgentMail, skills) overlaps with what you already use.

**What to try:** Pick two ideas to copy: the 7am PostHog funnel check that watches session replays when a step drops more than 10%, and the habit of turning every agent mistake into a skill. Also look at stablyai/orca and Lightpanda.

**Extra:** Mentions ideabrowser.com for idea and trend research.

[Open post](https://x.com/gregisenberg/status/2117734977312047537)
