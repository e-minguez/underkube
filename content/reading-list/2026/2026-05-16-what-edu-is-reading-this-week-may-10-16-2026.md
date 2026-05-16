---
title: "What Edu is reading this week (May 10 - 16, 2026)"
date: 2026-05-16T10:00:00+02:00
draft: false
slug: 2026-05-16-what-edu-is-reading-this-week-may-10-16-2026
aliases:
  - /posts/2026-05-16-what-edu-is-reading-this-week-may-10-16-2026/
categories:
  - Reading
tags:
  - newsletter
  - links
  - tech
  - devops
  - security
  - linux
  - ai
  - kubernetes
  - gaming
---

Busy week in AI agent land — Hermes Agent keeps growing, Anthropic's Mythos finds a real CVE in curl, and dnsmasq ships fixes for six serious vulnerabilities. Also: Faraday cages busted, a GPU-rendered terminal with a spinning rat, and the Mac clock project gets a proper full-length video.

![What Edu is reading this week (May 10 - 16, 2026)](/images/2026-05-16-what-edu-is-reading-this-week-may-10-16.png)

## AI, Agents & Tools

* [**NousResearch/hermes-agent**](https://github.com/nousresearch/hermes-agent) / [**I Switched from OpenClaw to Hermes Agent**](https://medium.com/@sathishkraju/i-switched-from-openclaw-to-hermes-agent-heres-what-nobody-told-me-5f33a746b6ca): Hermes Agent hit 110k GitHub stars in ten weeks — the fastest-growing agent framework of 2026, billed as "the agent that grows with you." The Medium piece breaks down what actually differentiates it from OpenClaw in practice.
* [**google-labs-code/design.md**](https://github.com/google-labs-code/design.md): A format spec for describing a visual identity to coding agents — gives agents a persistent, structured understanding of a design system via a `DESIGN.md` file. Same idea as CLAUDE.md, but for design.
* [**Friends Don't Let Friends Use Ollama**](https://sleepingrobots.com/dreams/stop-using-ollama/): Full history of Ollama — from riding llama.cpp's engine and dodging attribution, to VC money and a cloud pivot. The alternatives section alone is worth the read.
* [**l-mb/claude-code-redaction-hooks**](https://github.com/l-mb/claude-code-redaction-hooks): Claude Code hooks that scrub secrets and PII before they reach the API — a useful containment layer for agentic coding sessions.
* [**OWASP/secure-agent-playbook**](https://github.com/OWASP/secure-agent-playbook): OWASP's security playbook for AI agents — threat models, controls, and best practices for the agentic era.
* [**Mythos finds a curl vulnerability**](https://daniel.haxx.se/blog/2026/05/11/mythos-finds-a-curl-vulnerability/): Anthropic's Mythos model (not yet public due to its security-research capabilities) found a real vulnerability in curl. Daniel Stenberg documents the disclosure firsthand.
* [**Here is the current "Free-Tier AI Stack" for 2026**](https://www.reddit.com/r/AI_Agents/comments/1t97zn9/here_is_the_current_freetier_ai_stack_for_2026/): Reddit thread cataloguing free-tier options across frontier AI providers — Gemini at 1.5B tokens/day is the headline number, with a full breakdown of the rest.
* [**9 Principles That Separate Useful Skills from Markdown Essays**](https://generativeprogrammer.com/p/9-principles-that-separate-useful): A framework for designing Claude Code skills that fire at the right time, run correctly, and survive over time — practical rather than theoretical.

## Security

* [**Dnsmasq — Security IMPORTANT**](https://lists.thekelleys.org.uk/pipermail/dnsmasq-discuss/2026q2/018471.html): CERT disclosed six serious vulnerabilities in dnsmasq on May 11. If you're running it anywhere — embedded, homelab, anywhere — patch now.
* [**YellowKey — BitLocker Bypass Vulnerability**](https://github.com/Nightmare-Eclipse/YellowKey): Proof-of-concept BitLocker bypass — worth reading if you rely on BitLocker for encryption at rest.
* [**Air-gapped servers behind Faraday cages aren't safe from key exfiltration**](https://x.com/i/status/2053477658676380046): Researchers extracted data from a shielded, air-gapped machine using low-frequency magnetic fields, which pass straight through Faraday cages. Fake workloads encode the signal.
* [**The Cognitive Dark Forest**](https://ryelang.org/blog/posts/cognitive-dark-forest/): The open web with AIs is turning into a dark forest — an essay on signal decay, trust collapse, and what it means when you can't tell who's real anymore.

## Cloud, Kubernetes & Infrastructure

* [**Top 30 Argo CD Anti-Patterns to Avoid When Adopting GitOps**](https://octopus.com/blog/30-argo-cd-antipatterns-for-gitops): Solid catalog of common Argo CD mistakes that cause slowdowns and developer frustration — worth a pass before or after an adoption.
* [**New homelab router for 2026 recommendations**](https://forum.openwrt.org/t/new-homelab-router-for-2026-recomendations/249882/19): OpenWrt forum thread on homelab routing hardware for 2026 — discussion goes up to 4×2.5GbE + 2×10GbE Intel Core appliances for the serious end of the market.

## Linux & Systems

* [**Ratty**](https://ratty-term.org/): GPU-rendered terminal emulator with a spinning rat cursor, multiple 3D presentation modes, and inline 3D graphics. Built with Rust and Ratatui, explicitly inspired by TempleOS.
* [**oxidecomputer/skepsis**](https://github.com/oxidecomputer/skepsis): Local web UI for code review from Oxide Computer — no GitHub dependency, runs on your machine.
* [**So you've installed `fzf`. Now what?**](https://andrew-quinn.me/fzf/): Practical guide to getting real value out of fzf beyond the default shell history search.
* [**A Constructive Look At TempleOS**](http://www.codersnotes.com/notes/a-constructive-look-at-templeos/): Technical examination of TempleOS that takes the engineering seriously — what's genuinely interesting in the codebase, set aside from everything else.

## Gaming, Fun & Misc

* [**I turned a CLOCK into a vintage Mac!**](https://www.youtube.com/watch?v=dRr5iVjMfqs) / [**Fully Functioning Byte Sized Macintosh Plus**](https://www.youtube.com/shorts/L8BmkLJNtmA): Full video and short for the Maclock project — converting an AliExpress Mac-shaped desk clock into a working Macintosh with VNC, SSH, FTP, and Bluetooth keyboard support.
* [**Game Recommendations : r/PlaydateConsole**](https://www.reddit.com/r/PlaydateConsole/comments/1tcgshh/game_recommendations/): Community thread of must-buy Playdate games — useful if yours just arrived or is on the way.
* [**Boot Videos — Steam Deck Repo**](https://steamdeckrepo.com/): Community repository for custom Steam Deck startup movies, boot videos, and suspend animations.
* [**Setting up a free *.city.state.us locality domain**](https://fredchan.org/blog/locality-domains-guide/): In the US you can claim a free `somename.city.state.us` domain — this guide covers the Amazon Lightsail nameserver setup and the delegation request to the locality manager.
* [**BSD-NL Conference Early 2026 — On DOS, floppies, NetBSD and nostalgia**](https://exquisite.tube/w/dkV6kWiT9sp2y6xVwkH1iF): Conference talk covering retro DOS computing, floppy disks, NetBSD, and nostalgia — pleasant viewing.
