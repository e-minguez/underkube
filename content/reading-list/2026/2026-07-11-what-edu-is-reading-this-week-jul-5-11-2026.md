---
title: "What Edu is reading this week (Jul 5 - 11, 2026)"
date: 2026-07-11T10:00:00+02:00
draft: false
slug: 2026-07-11-what-edu-is-reading-this-week-jul-5-11-2026
aliases:
  - /posts/2026-07-11-what-edu-is-reading-this-week-jul-5-11-2026/
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

A week of DIY NAS builds and ZFS tooling, new frontier model releases from OpenAI and xAI, clever local inference tricks, and a couple of serious virtualization and AI-agent security stories.

![What Edu is reading this week (Jul 5 - 11, 2026)](/images/2026-07-11-what-edu-is-reading-this-week-jul-5-11.png)

## AI, Models & Agents

* [**GPT-5.6: Frontier intelligence that scales with your ambition**](https://openai.com/index/gpt-5-6/): OpenAI's latest release, pitched on more intelligence per token and stronger performance per dollar.
* [**Introducing Grok 4.5**](https://x.ai/news/grok-4-5): xAI's smartest model yet, built for coding, agentic tasks, and knowledge work.
* [**Introducing the OpenClaw Foundation**](https://openclaw.ai/blog/introducing-openclaw-foundation): OpenClaw becomes a non-profit, with a full-time team and a mission to bring personal AI to everyone.
* [**JustVugg/colibri**](https://github.com/JustVugg/colibri): Run GLM-5.2 (744B MoE) on a 25GB-RAM consumer machine — pure C, zero dependencies, experts streamed from disk.
* [**MTPLX**](https://mtplx.com/) / [**youssofal/MTPLX**](https://github.com/youssofal/MTPLX): A free, open-source Mac app that runs local LLMs up to twice as fast using native MTP speculative decoding on Apple Silicon, no external drafter needed.
* [**teamchong/pxpipe**](https://github.com/teamchong/pxpipe): Cut Fable 5 token usage by rendering text context as images.
* [**stefanprodan/cctop**](https://github.com/stefanprodan/cctop): A live top-style monitor for Claude Code sessions.
* [**Repomix**](https://repomix.com/): Pack your entire codebase into AI-friendly formats for feeding to LLMs.
* [**langchain-ai/openwiki**](https://github.com/langchain-ai/openwiki): A CLI that writes and maintains agent documentation for your codebase.

## Cloud, Kubernetes & Infrastructure

* [**mihaigalos/git-change-operator**](https://github.com/mihaigalos/git-change-operator): A Kubernetes operator for syncing resources or query results to Git via GitCommit/PullRequest custom resources.
* [**menlocloud/stratos**](https://github.com/menlocloud/stratos): A multi-tenant billing and self-service portal for OpenStack clouds, with a Go API and built-in AI agent integration via MCP.
* [**Zuck saves Meta bucks by reusing memory from old servers with a custom CXL ASIC**](https://www.theregister.com/systems/2026/06/29/zuck-saves-meta-bucks-by-reusing-memory-from-old-servers-with-a-custom-cxl-asic/5263483) / [**Panmnesia boosts CXL scale with fabric switching**](https://www.blocksandfiles.com/architecture/2026/06/26/panmnesia-boosts-cxl-scale-with-fabric-switching-meta-repurposes-old-dram-with-cxl/5263151): Meta repurposes DRAM from decommissioned servers via a custom CXL ASIC — in production on millions of boxes with a 25% reduction in machines for some inference workloads.

## NAS, Storage & Homelab

* [**NASdisks**](https://www.nasdisks.com/es/): Filter currently-sold NAS hard drives by CMR/SMR, capacity, class and real-world failure rates from Backblaze data.
* [**OpenZFS Capacity Calculator**](https://jro.io/capacity/): Plan your pool layout and see usable capacity for different RAIDZ configurations.
* [**Building a custom NAS with Fedora CoreOS**](https://xyny.art/blog/2026-building-nas/): A free NAS build with used disks and parts from a previous PC, running on Fedora CoreOS.
* [**How to Build a Minimal ZFS NAS without Synology, QNAP, TrueNAS**](https://neil.computer/notes/how-to-setup-minimal-zfs-nas-without-truenas/): If you don't care about GUI features, it is surprisingly simple to set up a ZFS dataset and share it over Samba.
* [**DIY NAS on NixOS**](https://www.splitbrain.org/blog/2025-08/03-diy_nas_on_nixos): Another take on the DIY NAS, this time declaratively configured with NixOS.
* [**kldload — pick your distro, get ZFS on root**](https://kldload.com/zfs-wiki/myths): One ISO that installs CentOS, Debian, Ubuntu, Fedora, RHEL, Rocky, Arch or FreeBSD with ZFS on root, WireGuard and eBPF — offline and free.
* [**10 Cheap AliExpress Zigbee Smart Buttons Tested**](https://smarthomescene.com/reviews/aliexpress-zigbee-smart-buttons-tested/): The ten cheapest Zigbee smart buttons from AliExpress, tested for latency, build quality and Zigbee performance.

## Linux & Systems

* [**'I'm not a programmer' anymore: Linus Torvalds on the only two tools he uses now**](https://www.zdnet.com/article/open-source-summit-linus-torvalds/): Torvalds at the Open Source Summit in Mumbai on the pain and power of AI in the kernel, and why Linux no longer supports "museum" technology.
* [**Interview With Mitchell Hashimoto**](https://alexalejandre.com/programming/interview-with-mitchell-hashimoto/): The Ghostty and Terraform maker and HashiCorp founder talks about open source, terminals and Zig.
* [**Hannah Montana Linux gets modern remaster after nearly two decades**](https://www.tomshardware.com/software/linux/hannah-montana-linux-gets-modern-remaster-after-nearly-two-decades-sweet-niblets-new-v26-is-built-on-debian-with-a-re-skin-of-kde-plasma): The new v26 is built on Debian with a re-skin of KDE Plasma — a chance to catch up with 18 years of security patches.
* [**T00fy/omanix**](https://github.com/T00fy/omanix): A NixOS module inspired by Omarchy.
* [**News about Linux (Crostini) on ChromeOS**](https://developers.google.com/chromeos/app-development/develop/news): Google's news feed for Linux development environments on ChromeOS.
* [**b-aaz/bmake-extravaganza**](https://github.com/b-aaz/bmake-extravaganza): Pushing BSD-make to places it was not designed for.
* [**MacSurf — the modern web, on a 25-year-old Mac**](https://macsurf.org/): A real web browser for Classic Mac OS 9 PowerPC — CSS3, modern JavaScript and native HTTPS, built with CodeWarrior on the Carbon API.
* [**Davit — a native macOS UI for Apple containers**](https://davit.app): Free, open-source and fully native — run Linux containers on Apple silicon with Apple's container platform, no Docker Desktop required.

## Security

* [**16-Year-Old Linux KVM Flaw Lets Guest VMs Escape to Host**](https://thehackernews.com/2026/07/16-year-old-linux-kvm-flaw-lets-guest.html): "Januscape" abuses KVM shadow MMU page reuse to panic x86 hosts on Intel and AMD, with a controlled full-escape exploit reported.
* [**CVE-2026-57589**](https://nvd.nist.gov/vuln/detail/cve-2026-57589): A use-after-free in OpenBSD's `sys_semget()` (through 7.9) allowing local privilege escalation to root — CVSS 7.8.
* [**Decades-Old Bash Tricks Expose AI Coding Agents To Supply Chain Attacks**](https://linux.slashdot.org/story/26/07/04/0325244/decades-old-bash-tricks-expose-ai-coding-agents-to-supply-chain-attacks): "GuardFall" uses shell behaviors like quote removal and variable expansion to bypass safeguards in most open-source AI coding agents.
* [**Red teamers turned Claude Desktop into a double agent**](https://www.theregister.com/security/2026/07/01/red-teamers-turned-claude-desktop-into-a-double-agent-to-do-their-evil-bidding/5264692): People trust their AI assistants, and it's easy to abuse this trust.

## Gaming, Fun & Misc

* [**Solo Dev's Train Sim Is Being Called The Best Ever Made**](https://kotaku.com/a-train-sim-created-by-just-one-person-is-being-called-the-best-ever-made-2000699429): Steam reviews are blowing up for Running Train, a gorgeous Japanese train driving simulator made by one person.
* [**Quakeworld Air Physics**](https://mattias.niklewski.com/2013/01/qw_air_physics.html): A classic write-up on the math behind QuakeWorld's air movement — why bunny-hopping and strafe-jumping work the way they do.
* [**Can you run every line of code in Super Mario Bros.?**](https://www.youtube.com/watch?v=o0gOALTvkcc): An attempt to execute every line of code in Super Mario Bros., including bytes inaccessible under normal play.
* [**MaximeRivest/riddle**](https://github.com/MaximeRivest/Riddle): The diary of Tom Riddle for the reMarkable Paper Pro — write with your pen, the page drinks your ink and answers in a flowing hand.
* [**An obfuscated bash script on a Uniqlo t-shirt**](https://tris.sherliker.net/blog/obfuscated-self-evaluating-bash-script-by-cdn-akamai-being-supplied-to-consumers-via-retail-stores/): Decoding the self-evaluating bash script printed on a Uniqlo x Akamai t-shirt — it turns out to be an animated "Peace for All" easter egg.
* [**Ubisoft Barcelona Celebrates Successful Assassin's Creed Black Flag Resynced Launch With Layoffs**](https://insider-gaming.com/assassins-creed-black-flag-resynced-layoffs/): 51 employees, many of whom worked on the remake, laid off right after launch.
