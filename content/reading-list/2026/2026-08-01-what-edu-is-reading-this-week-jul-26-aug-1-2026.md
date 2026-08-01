---
title: "What Edu is reading this week (Jul 26 - Aug 1, 2026)"
date: 2026-08-01T10:00:00+02:00
draft: false
slug: 2026-08-01-what-edu-is-reading-this-week-jul-26-aug-1-2026
aliases:
  - /posts/2026-08-01-what-edu-is-reading-this-week-jul-26-aug-1-2026/
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
  - hardware
  - gaming
---

A week of running LLM inference on your own Kubernetes clusters, a Secure Boot bypass that went unnoticed for a decade, terminal demo tooling, UPS dashboards and plenty of retro hardware. This is the last post for a while: I'm off on holidays, so the newsletter takes a break and will be back once I'm home.

## AI, Models & Agents

* [**The real AI risk is inside the labs**](https://antirez.com/news/172): antirez argues the main risk is not open models or international competition, but a handful of unelected lab executives making hard choices for everyone else.
* [**Our position on open-weights models**](https://www.anthropic.com/news/position-open-weights-models): Anthropic's Dario Amodei on how the company sees open-weights models.
* [**Bifrost AI Gateway**](https://docs.getbifrost.ai/overview): A high-performance AI gateway unifying 20+ providers behind a single OpenAI-compatible API, with failover so applications keep serving.
* [**drumih/turbo-fieldfare**](https://github.com/drumih/turbo-fieldfare): Gemma 4 26B-A4B inference in roughly 2 GB of RAM on any M-series MacBook.
* [**Qué GPU necesitas para servir modelos de IA**](https://helmcode.com/es/posts/gpu-families-precision-hardware): In Spanish — FP8 and NVFP4, what each NVIDIA generation accelerates in hardware, how much VRAM your model needs and which GPU to buy, with production data.
* [**The first real desktop written by AI**](https://starling.build/?ref=selfh.st): A complete Linux desktop — compositor, window manager, Wayland and X11 servers, apps — written by AI and directed by one person over six months.
* [**DrewThomasson/ebook2audiobook**](https://github.com/DrewThomasson/ebook2audiobook): Generate audiobooks from e-books with voice cloning and support for 1158+ languages.
* [**Professor's invisible prompt trap catches 32 students cheating on their midterm with AI**](https://www.techspot.com/news/113243-professor-invisible-prompt-trap-catches-32-students-cheating.html): A history professor hid an instruction inside an online discussion prompt and 32 submissions dutifully followed it.

## Cloud, Kubernetes & Infrastructure

* [**In-house LLM Inference on Kubernetes: A Production Runbook**](https://gd03.me/writings/inference-infra) / [**Karpenter**](https://karpenter.sh/) / [**KEDA**](https://keda.sh/): The actual runbook for standing up in-house inference on EKS — GPU nodes with Karpenter, vLLM under llm-d, event-based autoscaling on serving metrics with KEDA, and the economics behind it.
* [**Prometheus Monitoring Mixins**](https://monitoring.mixins.dev/): Grafana dashboards plus Prometheus rules and alerts packaged into reusable, extensible bundles written in jsonnet and installed with jsonnet-bundler.
* [**Stacked pull requests are now in public preview**](https://github.blog/changelog/2026-07-30-stacked-pull-requests-are-now-in-public-preview/): GitHub adds stacks — an ordered series of small pull requests that each represent a focused layer of a larger change.

## Security

* [**Microsoft's Secure Boot has been broken for a decade and no one noticed until now**](https://arstechnica.com/security/2026/07/microsoft-secure-boot-has-been-broken-for-most-of-its-existence/) / [**CERT/CC VU#616257**](https://kb.cert.org/vuls/id/616257): Old Microsoft-signed UEFI shims that were never revoked make Secure Boot bypasses straightforward, with the CERT/CC note tracking affected vendors.
* [**Stronger with every update: How we're making Chrome and the web safer in the AI Era**](https://blog.google/security/chrome-stronger-with-every-update/): Google describes using Gemini to automate vulnerability discovery, triage and patching in Chrome.
* [**openai/codex-security**](https://github.com/openai/codex-security): OpenAI's Codex Security CLI and TypeScript SDK for finding, validating and fixing security vulnerabilities.
* [**About the security content of macOS Tahoe 26.6**](https://support.apple.com/en-us/128067): Apple's list of what got fixed in the latest macOS release.

## Linux & BSD

* [**Setup a Simple, Self-Hosted Web Server with OpenBSD**](https://btxx.org/posts/self-hosted-openbsd/): Setting up a simple, self-hosted web server with OpenBSD.
* [**I Built a FreeBSD Cloud to Use with FreeBSD**](https://interfacecraft.online/blog/2026/i-built-a-freebsd-cloud-to-use-with-freebsd/): Rolling your own file sync across devices on FreeBSD instead of renting a commercial cloud, keeping automation and privacy under your control.
* [**ftonneau/grub-evodevo**](https://github.com/ftonneau/grub-evodevo): A configurable GRUB theme with scalable graphics and smooth fonts.

## Self-Hosting & Homelab

* [**Dockhand**](https://dockhand.pro/#) / [**Finsys/hawser**](https://github.com/Finsys/hawser): A Docker management platform with real-time container management, Compose stacks, Git deployments and SSO, paired with Hawser, a lightweight Go agent that lets it manage hosts across different network setups.
* [**sablierapp/sablier**](https://github.com/sablierapp/sablier): Start containers on demand and shut them down when there is no activity — works with Docker, Swarm, Podman, Kubernetes and Proxmox LXC.
* [**Diun**](https://crazymax.dev/diun/): Get notified when a Docker image you depend on is updated in its registry.
* [**Brandawg93/PeaNUT**](https://github.com/Brandawg93/PeaNUT) / [**DartSteven/Nutify**](https://github.com/DartSteven/Nutify): Two web dashboards for Network UPS Tools — one tiny and minimal, one with real-time visualisation, alerts and reporting.
* [**Jailbroken Kindles can now do more with Tailscale**](https://tailscale.com/blog/jailbroken-kindle-proxy-tun-modes): Community updates bring Tailscale SSH, proxy modes for KOReader and full TUN mode to jailbroken Kindles, plus plugins for Kobo and Pocket Reader.

## Development, Web & Tools

* [**mfontanini/presenterm**](https://github.com/mfontanini/presenterm): Give slide decks straight from markdown in your terminal.
* [**charmbracelet/vhs**](https://github.com/charmbracelet/vhs): Script terminal recordings as code and render them to GIF — your CLI home video recorder.
* [**sloria/doitlive**](https://github.com/sloria/doitlive) / [**paxtonhare/demo-magic**](https://github.com/paxtonhare/demo-magic): Two takes on faking live typing so shell demos are repeatable and never fail on stage.
* [**vrtmrz/obsidian-livesync**](https://github.com/vrtmrz/obsidian-livesync) / [**siosig/obsidian-nextcloudsync**](https://github.com/siosig/obsidian-nextcloudsync): Self-hosted LiveSync syncs Obsidian across all platforms via CouchDB or object storage (MinIO, S3, R2), and can also go peer-to-peer over WebRTC with only a signalling relay; the second plugin does the same against Nextcloud.
* [**itsfatduck/optimizerDuck**](https://github.com/itsfatduck/optimizerDuck): A free, open-source Windows optimisation tool aimed at performance, privacy and simplicity.

## Hardware, Retro & Gaming

* [**Thimbleweed Park 2**](https://www.grumpygamer.com/twp2_announce/): Ron Gilbert announces Thimbleweed Park 2 is being developed.
* [**Game Industry Hardship Fund Bundle**](https://itch.io/b/3802/game-industry-hardship-fund): 127 items for $10 from nearly 150 creators, with proceeds going to the United Videogame Workers hardship fund for out-of-work developers in North America.
* [**Half-Life ported to Mac OS 9**](https://mac-classic.com/news/half-life-ported-to-mac-os-9/): Half-Life ported to Mac OS 9, decades after the fact.
* [**Sega Game Gear Repair Reference**](https://consoleartisan.com/reference/game-gear/): Symptom-to-fix guide from someone who restores Game Gears — dead or dim screens, no sound, capacitor replacement and the region power-jack polarity.
* [**crazy-electron/gambatte-k2**](https://github.com/crazy-electron/gambatte-k2): A lightweight Game Boy / Color / Advance emulator frontend for Kindle e-ink devices, with grayscale rendering and Bluetooth headphone support.
* [**XayroWhite/UTUBBU**](https://github.com/XayroWhite/UTUBBU): An unofficial YouTube client for the PSP.
* [**stshunz/WProton**](https://github.com/stshunz/WProton): A portable Windows game launcher for Linux that runs games via Proton or Wine, with gamepad-navigable menus and bundled runners and prefixes.
* [**hrvach/deskhop**](https://github.com/hrvach/deskhop): Share one keyboard and mouse between two computers, switching with a shortcut or by moving the pointer between monitors — no clumsy USB box, and it works across different operating systems.

## Fun & Misc

* [**ShitCode**](https://shitcode.org/) / [**RUIN.MEDIA**](https://shitcode.org/Korosys/RUIN.MEDIA): A GitHub-style forge with a twist — the best place for your dumpsterfire code — hosting things like RUIN.MEDIA, a Docker-based PHP app for reducing the quality of images and audio.
* [**Don't use 🥞 as menu icon**](https://github.com/orgs/community/discussions/203497): A GitHub community discussion objecting, at length, to pancakes replacing the hamburger menu.
* [**Too Tired to Game | Surviving the Dad Fatigue Loop**](https://youtube.com/watch?v=A8xFKYwac8k&is=N7rtWIn37bzv307R): A video essay on the "Dad Fatigue Loop" — why the backlog turns into game shame when there is no energy left, and how to make fifteen minutes feel like enough instead of waiting for a two-hour window that never arrives.
* [**Magnolias Are So Old That They're Pollinated by Beetles**](https://mymodernmet.com/magnolia-ancient-flowers-beetles/): Magnolias predate bees, so beetles still do the pollinating.
</content>
