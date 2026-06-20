---
title: "What Edu is reading this week (Jun 14 - 20, 2026)"
date: 2026-06-20T07:00:00+02:00
draft: false
slug: 2026-06-20-what-edu-is-reading-this-week-jun-14-20-2026
aliases:
  - /posts/2026-06-20-what-edu-is-reading-this-week-jun-14-20-2026/
categories:
  - Reading
tags:
  - newsletter
  - links
  - tech
  - devops
  - linux
  - ai
  - security
  - selfhosted
---

A week heavy on local LLM coding setups, token-trimming tooling, dotfile managers, ZFS self-hosting, and a couple of supply-chain security reminders.

![What Edu is reading this week (Jun 14 - 20, 2026)](/images/2026-06-20-what-edu-is-reading-this-week-jun-14-20.png)

## Local AI & Coding Agents

* [**Running local models is good now**](https://vickiboykis.com/2026/06/15/running-local-models-is-good-now/) / [**Ask HN: Has anyone replaced Claude/GPT with a local model?**](https://news.ycombinator.com/item?id=48542100): Vicki Boykis argues local agentic coding has become genuinely good over the past few months, alongside the Hacker News thread of people sharing their daily-driver local setups.
* [**How to Setup a Local Coding Agent on macOS**](https://ikyle.me/blog/2026/how-to-setup-a-local-coding-agent-on-macos): Running Gemma 4 26B-A4B and Qwen3.6 35B-A3B locally with llama.cpp, MTP speculative decoding, and multimodal support as a coding agent.
* [**Running a Local LLM Coding Server on MacBook Pro M5 Pro 48 GB**](https://blog.kulman.sk/running-local-llm-coding-server/): An honest account of running a local coding AI on Apple Silicon — what crashed, what worked, and why the author settled on Ollama with Qwen 3.6 MoE.
* [**crim50n/oc-remote**](https://github.com/crim50n/oc-remote): An Android client for OpenCode servers, for driving your coding agent from a phone.
* [**Fusion — OpenRouter**](https://openrouter.ai/openrouter/fusion): Turns a single prompt into a small multi-model deliberation, with a 128K context window.

## AI Tooling

* [**yvgude/lean-ctx**](https://github.com/yvgude/lean-ctx) / [**chopratejas/headroom**](https://github.com/chopratejas/headroom): Two takes on cutting agent token usage — LeanCTX is a local Rust binary that controls what an agent reads and remembers, while Headroom compresses tool outputs, logs, and RAG chunks before they reach the LLM, both claiming 60-95% fewer tokens.
* [**alibaba/open-code-review**](https://github.com/alibaba/open-code-review): A hybrid code review tool combining deterministic pipelines with an LLM agent for line-level comments, with a built-in ruleset for NPE, thread-safety, XSS, and SQL injection.
* [**Gentleman-Programming/gentle-ai**](https://github.com/Gentleman-Programming/gentle-ai): Not an agent installer but an ecosystem configurator — it supercharges whatever coding agent you use (Claude Code, OpenCode, Cursor) with persistent memory, Spec-Driven Development workflows, curated skills, MCP servers, an AI provider switcher, a security-first teaching persona, and per-phase model assignment so each SDD step can run on a different model.
* [**mge1512/pcd**](https://github.com/mge1512/pcd): Post-Coding Development ("Piccadilly") — the specification, not source code, is the human deliverable. A structured Markdown spec captures what software must do and an LLM produces the implementation, tests, docs, and audit bundle; the target language is chosen by the deployment template, so the same untouched spec could yield a Go binary today and a Rust one in 2045. The repo's own reference tools were generated from PCD specs with zero hand-written code.
* [**AI Economics for Dummies**](https://www.mcsweeneys.net/articles/ai-economics-for-dummies): McSweeney's satirical word problem on the economics of running an AI business at a multi-billion-dollar monthly loss.

## Cloud, Containers & Infrastructure

* [**apple/containerization — kernel**](https://github.com/apple/containerization/tree/main/kernel): The kernel directory of Apple's Swift package for running Linux containers on macOS.
* [**macgaver/zfsnas-chezmoi (ZNAS)**](https://github.com/macgaver/zfsnas-chezmoi): A NAS management UI built on ZFS.
* [**whoschek/bzfs**](https://github.com/whoschek/bzfs): A CLI for reliable, scalable near real-time ZFS snapshot replication using `zfs send/receive` and ssh, able to operate at sub-second intervals across large fleets.
* [**Hetzner increased dedicated server prices 3-4x**](https://news.ycombinator.com/item?id=48542064): Hacker News discussion on Hetzner's dedicated server price hikes and the alternatives people are weighing.

## Linux & Systems

* [**Migrating from GNU stow to chezmoi**](https://rednafi.com/misc/chezmoi/) / [**Yet Another Dotfiles Manager (yadm)**](https://yadm.io/#): Why one developer swapped stow's symlink farm for chezmoi's one-command bootstrap, plus yadm as another git-based dotfiles manager.
* [**Making HTTP requests from a container that has no curl, using bash /dev/tcp**](https://mareksuppa.com/til/bash-dev-tcp-http-without-curl/): Minimal container images often ship without any HTTP client — Bash can open a TCP socket through `/dev/tcp` to hand-write a tiny HTTP/1.1 request for quick checks.
* [**XuehaiPan/nvitop**](https://github.com/XuehaiPan/nvitop): An interactive NVIDIA-GPU process viewer and one-stop GPU process manager.
* [**FreeBSD 15 on a Laptop**](https://www.reddit.com/r/freebsd/s/xGCD2Ssiz6): A report on daily-driving FreeBSD 15 as a laptop OS.
* [**ReactOS reaches the milestone of running Half-Life**](https://www.phoronix.com/news/ReactOS-Running-Half-Life): The open-source Windows-compatible OS can now run the classic Half-Life.
* [**s0xDk/ghostty-blackhole**](https://github.com/s0xDk/ghostty-blackhole): Puts a real, ray-traced black hole inside your terminal that grows live as Claude Code's context window fills — a fresh session is a quiet hole in the corner, a full one swallows half your screen, so you always see `/compact` coming.

## Security

* [**A backdoor in a LinkedIn job offer**](https://roman.pt/posts/linkedin-backdoor/): A fake recruiter, a crypto repo, and a remote code execution payload hidden in a test file.
* [**Hundreds of AUR packages compromised**](https://lwn.net/Articles/1077718/): Hundreds of orphaned packages on the Arch User Repository were compromised, a reminder of the trust model behind community repos.
* [**curl summer of bliss**](https://daniel.haxx.se/blog/2026/06/15/curl-summer-of-bliss/): The curl project will pause vulnerability report handling for the month of July 2026 to give maintainers a break.
* [**NVIDIA/SkillSpector**](https://github.com/NVIDIA/SkillSpector): A security scanner for AI agent skills, detecting vulnerabilities and malicious patterns.
* [**Banned Book Library**](https://www.richardosgood.com/posts/banned-book-library/): Hacking a WiFi smart bulb into a hidden device that serves a library of banned books.

## Development, Web & Fun

* [**Mechanical Watch — Bartosz Ciechanowski**](https://ciechanow.ski/mechanical-watch/): An interactive article explaining how a mechanical watch works, in classic Ciechanowski style.
* [**Bubbles**](https://bubbles.town/): Independent blog posts ranked by the community — good stuff bubbles up, the rest pops.
* [**Motherfucking Website**](https://motherfuckingwebsite.com/): A reminder that a website really does not need much.
* [**Spencer Baggins on the French engineer the internet runs on**](https://x.com/bigaiguy/status/2063903532575752211): A thread on the quiet Paris engineer (Fabrice Bellard) whose code streams every YouTube, Netflix, and TikTok clip and runs countless virtual machines.

## Gaming, Fun & Misc

* [**putt.day**](https://putt.day/): One hole of mini golf a day — the same hole for everyone.
* [**Flip-Phone — Commodore**](https://commodore.net/callback/): A smarter flip phone with no social media, from Commodore.
* [**Subterranean fungi networks more than 100 quadrillion km in length**](https://www.theguardian.com/science/2026/jun/11/arbuscular-mycorrhizal-fungi-plant-life-climate-global-mapping-study): The first global mapping of arbuscular mycorrhizal fungi reveals the scale of the underground hyphal systems that sustain plant life.
