---
title: "What Edu is reading this week (Jul 12 - 18, 2026)"
date: 2026-07-18T08:00:00+02:00
draft: false
slug: 2026-07-18-what-edu-is-reading-this-week-jul-12-18-2026
aliases:
  - /posts/2026-07-18-what-edu-is-reading-this-week-jul-12-18-2026/
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
  - sdr
  - gaming
---

A week of new open frontier models and AI CLI wire-level analysis, a 15-year-old Linux kernel privilege escalation, ZFS and FreeBSD tooling, plus plenty of hardware, SDR and retro-computing rabbit holes.

## AI, Models & Agents

* [**Kimi K3 Tech Blog: Open Frontier Intelligence**](https://www.kimi.com/blog/kimi-k3): Moonshot's tech blog for its Kimi K3 model, pitched as open frontier intelligence.
* [**Announcing Bonsai 27B: The First 27B-Class Model to Run on a Phone**](https://prismml.com/news/bonsai-27b): PrismML's Bonsai 27B, presented as the first 27B-class model that runs on a phone.
* [**What xAI Grok Build CLI actually sends to xAI — a wire-level analysis**](https://gist.github.com/cereblab/dc9a40bc26120f4540e4e09b75ffb547#what-xais-grok-build-cli-actually-sends-to-xai-a-wire-level-analysis): A wire-level look at exactly what the xAI Grok Build CLI (grok 0.2.93) transmits back to xAI.
* [**Claude Code Sends 4.7x More Tokens Than OpenCode Before Reading Your Prompt**](https://systima.ai/blog/claude-code-vs-opencode-token-overhead) / [**Discussion**](https://news.ycombinator.com/item?id=48883275): Measuring what Claude Code and OpenCode spend before reading your prompt, then adding instruction files, MCP servers and subagents to the bill.
* [**Musheer360/SwiftSlate**](https://github.com/Musheer360/SwiftSlate): An Android accessibility service for AI-powered text transformation.
* [**Clawptcha — Reverse CAPTCHA for Bots & AI Agents**](https://clawptcha.com/): A reverse CAPTCHA that proves you're a bot, not a human — for AI agents and automated systems.

## Cloud, Kubernetes & Infrastructure

* [**containers/kubernetes-mcp-server**](https://github.com/containers/kubernetes-mcp-server): A Model Context Protocol (MCP) server for Kubernetes and OpenShift.
* [**SELinux Volume Label Changes goes GA (and likely implications in v1.37)**](https://kubernetes.io/blog/2026/04/22/breaking-changes-in-selinux-volume-labeling/): If you run Kubernetes on Linux with SELinux enforcing, plan ahead — the SELinuxMount gate is expected on by default around v1.37, which speeds up volume setup but can break apps relying on recursive relabeling.
* [**gpubox**](https://ericcurtin.github.io/gpubox/blog/2026-07-15-introducing-gpubox.html) / [**ericcurtin/gpubox**](https://github.com/ericcurtin/gpubox): An auto-detecting, GPU-aware container launcher.
* [**Dependabot version updates introduce default package cooldown**](https://github.blog/changelog/2026-07-14-dependabot-version-updates-introduce-default-package-cooldown/): Dependabot now waits until a new release has been on its registry for at least three days before opening a version update PR.

## Linux & Systems

* [**FreeBSD 16 Retires The Last Of Its GPL Code From Its Base System**](https://www.phoronix.com/news/FreeBSD-16-Goes-GPL-Free): As of this past week in the FreeBSD 16 source tree, the last of the GNU GPL-licensed code has been retired from the base system.
* [**topgrade-rs/topgrade**](https://github.com/topgrade-rs/topgrade): One command to upgrade all the things across your system's package managers and tools.
* [**Re: Linking Patchwork with Sashiko**](https://lore.kernel.org/linux-media/CAHk-=wi4zC+Ze8e+p3tMv8TtG_80KzsZ1syL9anBtmEh5Z40vg@mail.gmail.com/): Linus Torvalds puts his foot down on the linux-media list — "Linux is not one of those anti-AI projects." Over a proposal to wire Patchwork's patch tracking to Sashiko (an AI bug-finding tool for kernel patches), he says no one is forced to use AI, but he'll loudly ignore anyone trying to stop others from adopting it.
* [**Block Cloning in ZFS**](https://slicker.me/zfs/block-cloning.html): A technical reference for ZFS block cloning — the Block Reference Table, trigger paths, requirements, tunables, stability history and `zfs send/receive` interaction.
* [**ArthorH/Ubuntu-ZFS-Install-existing-pool**](https://github.com/ArthorH/Ubuntu-ZFS-Install-existing-pool): An Ubuntu zfsbootmenu install onto an existing ZFS pool, without formatting or editing existing partitions.
* [**lobste.rs is now running on SQLite**](https://lobste.rs/s/ko1ji1/lobste_rs_is_now_running_on_sqlite): The community link aggregator has migrated its database to SQLite.
* [**8 Linux Handheld Computers You Can Splurge On**](https://itsfoss.com/linux-handhelds/): A roundup of Linux handhelds that are ready to use out of the box, no spare Raspberry Pi or tinkering required.

## Security

* [**IonStack part II: GhostLock, a stack-UAF that has existed in ALL Linux distributions for 15 years**](https://nebusec.ai/research/ionstack-part-2/): GhostLock (CVE-2026-43499) is a Linux kernel bug present in every major distribution since 2011, turned into a 97%-stable privilege escalation and container escape — earning $92,337 in kernelCTF.

## Development, Web & Tools

* [**Visual Studio Code 1.129**](https://code.visualstudio.com/updates/v1_129#_modern-ui-preview-experimental): What's new in VS Code 1.129, including an experimental Modern UI preview.
* [**cachix/secretspec**](https://github.com/cachix/secretspec): Declarative secrets for every environment and any provider.
* [**Microsoft Comic Chat is now open source**](https://opensource.microsoft.com/blog/2026/07/16/microsoft-comic-chat-is-now-open-source/): The IRC client that turned conversations into comics — and helped introduce Comic Sans to the world — has been open sourced.
* [**Never Argue With Your Boss (2009)**](https://righteousit.com/2009/03/12/never-argue-with-your-boss/) / [**Discussion**](https://news.ycombinator.com/item?id=48861184): A career-advice classic on "managing your manager", from a talk by Bill Howell.

## SDR, Hardware & Electronics

* [**Teardown: A Generic 7-Port USB 3.0 Hub That Wasn't**](https://goughlui.com/2026/07/09/teardown-a-generic-7-port-usb-3-0-hub-that-wasnt/): An AliExpress bargain USB 3.0 hub gets taken apart — and turns out to be not quite what the listing promised.
* [**The Scariest Chart In Electrical Engineering**](https://www.youtube.com/watch?v=GK2pZ_oVU1o): Veritasium on why the Smith Chart has such a fearsome reputation among electrical engineers.
* [**darrylmorley/whatcable**](https://github.com/darrylmorley/whatcable) / [**The Verge**](https://www.theverge.com/gadgets/963759/whatcable-usb-c-cable-tester-app-mac): A free macOS menu bar app (M1 or later) that tells you, in plain English, what each USB-C cable plugged into your Mac can actually do.
* [**vjsoriano83/onu-sfp-alcatel-lucent-setup**](https://github.com/vjsoriano83/onu-sfp-alcatel-lucent-setup): Setup notes for an Alcatel-Lucent ONU SFP module.
* [**Quansheng UV-K5 Wiki**](https://github.com/ludwich66/Quansheng_UV-K5_Wiki/wiki) / [**Multi-UVTools**](https://spm81.github.io/Multi-UVTools/#instructions): Firmware wiki and multi-tool flashing instructions for the popular Quansheng UV-K5 handheld radio.

## Networking

* [**Mysteries of Telegram DC**](https://dev.moe/en/3025): A dig into Telegram's five data centers — where they are, how accounts get assigned, and the quirks around them.
* [**Telegram's t.me domain has been suspended**](https://news.ycombinator.com/item?id=48897878): Hacker News discussion on the suspension of Telegram's t.me domain.
* [**I co-founded pfSense. For the last year I've been building its successor.**](https://x.com/i/status/2075771099812409605): A pfSense co-founder on the reasons to look beyond pfSense today — and the successor he's been building.

## Gaming, Fun & Misc

* [**dibdot/uWolf**](https://github.com/dibdot/uWolf) / [**OpenWrt Forum**](https://forum.openwrt.org/t/uwolf-your-router-now-runs-wolfenstein-3d/251797): A dependency-free JavaScript raycaster that reads the original Wolfenstein 3D data formats and renders them in the browser — served as static files by OpenWrt's uhttpd, so your router can now run Wolfenstein 3D.
* [**Bless The BC250, The Budget E-waste Steam Machine**](https://aftermath.site/bc250-steam-machine-budget-computer/): Building a miracle budget gaming computer out of cheap BC250 mining-rig garbage.
* [**Jurassic Park computers in excruciating detail**](https://fabiensanglard.net/jurrasic_park_computers/index.html): Fabien Sanglard dissects the real computers and software that appear in Jurassic Park.
* [**First atmosphere found around Earth-like planet LHS 1140b**](https://www.bbc.com/news/articles/cy4kdd1e0ejo): Researchers report an Earth-like rocky planet with an atmosphere orbiting within its star's habitable zone.
* [**Aymeric Laporte, first player to beat his country of birth in a World Cup semi-final**](https://www.reddit.com/r/interestingasfuck/comments/1ux1gyt/aymeric_laporte_has_become_the_first_ever_player/): He captained France at youth levels but switched to Spain after receiving citizenship in 2021 — and just beat France in a World Cup semi-final.
