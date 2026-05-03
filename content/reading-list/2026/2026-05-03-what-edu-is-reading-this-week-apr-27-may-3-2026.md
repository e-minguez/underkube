---
title: "What Edu is reading this week (Apr 27 - May 3, 2026)"
date: 2026-05-03T10:00:00+02:00
draft: false
slug: 2026-05-03-what-edu-is-reading-this-week-apr-27-may-3-2026
aliases:
  - /posts/2026-05-03-what-edu-is-reading-this-week-apr-27-may-3-2026/
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
---

Big week: a no-race, 100% reliable Linux LPE hitting all major distributions, a flood of AI agent sandboxing content, and another wave of Claude Code tooling.

![Reading list header image](/images/2026-05-03-what-edu-is-reading-this-week-apr-27-may-3.png)

## Security

* [**Copy Fail — CVE-2026-31431**](https://copy.fail/) / [**Copy Fail: 732 Bytes to Root**](https://xint.io/blog/copy-fail-linux-distributions): A 100% reliable Linux local privilege escalation exploiting AF_ALG + splice() for a 4-byte page cache write — no race condition, no per-distro offsets, bypasses on-disk file-integrity tools and crosses containers. A 732-byte PoC gets root on Ubuntu, Amazon Linux, RHEL, and SUSE.
* [**tgies/copy-fail-c**](https://github.com/tgies/copy-fail-c): Cross-platform C port of the Copy Fail PoC (CVE-2026-31431), disclosed by Theori / Xint on April 29.
* [**NorskHelsenett/copy-fail-destroyer**](https://github.com/NorskHelsenett/copy-fail-destroyer): Mitigation tooling for Copy Fail.
* [**GTFOBins**](https://gtfobins.org/): Curated list of Unix binaries exploitable to bypass local security restrictions in misconfigured systems — always useful.

## Cloud, Kubernetes & Infrastructure

* [**Kubernetes 1.36 UserNamespaces GA: great feature, dangerously oversold**](https://www.reddit.com/r/kubernetes/comments/1sytvxf/kubernetes_136_usernamespaces_ga_great_feature/): A grounded take on K8s 1.36 UserNamespaces reaching GA — what it actually protects and where the security boundary claims fall short.
* [**FOSDEM 2026 - All videos are online**](https://fosdem.org/2026/news/2026-04-26-all-videos-published/): All FOSDEM 2026 talks now available for streaming and download.
* [**microvm.nix**](https://microvm-nix.github.io/microvm.nix/) / [**microvm-nix/microvm.nix**](https://github.com/microvm-nix/microvm.nix): NixOS MicroVMs — lightweight VMs declaratively managed with Nix.
* [**nirs/vmnet-helper**](https://github.com/nirs/vmnet-helper) / [**nirs/vmnet-broker**](https://github.com/nirs/vmnet-broker): High-performance network proxy and shared XPC service for connecting VMs to macOS vmnet — useful for Apple Virtualization framework setups.
* [**Devbox**](https://www.jetify.com/devbox) / [**devenv**](https://devenv.sh/): Portable, isolated dev environments without Docker. Devbox uses Nix under the hood; devenv is declarative and composable. Two solid alternatives for reproducible local dev.
* [**Tracer-Cloud/opensre**](https://github.com/Tracer-Cloud/opensre): Open source toolkit for building AI SRE agents.

## AI, Agents & Tools

* [**What every dev should know about AI sandboxes**](https://read.engineerscodex.com/p/every-dev-should-know-about-ai-sandboxes) / [**A field guide to sandboxes for AI**](https://luiscardoso.dev/blog/sandboxes-for-ai): Two complementary reads on sandboxing for AI agents — containers vs gVisor vs microVMs vs Wasm, what each boundary buys you, and where they fail.
* [**Safe Yolo Mode: Running LLM Agents in VMs with Libvirt and Virsh**](https://www.metachris.dev/2026/02/safe-yolo-mode-running-llm-agents-in-vms-with-libvirt-and-virsh/): Give LLM agents full shell access inside a libvirt VM without risking the host — covers VM creation, snapshots, and remote access.
* [**lynaghk/vibe**](https://github.com/lynaghk/vibe): Easy Linux VM on macOS for sandboxing LLM agents.
* [**sylvinus/agent-vm**](https://github.com/sylvinus/agent-vm/tree/main): Run AI agents in safe VMs scoped to a local folder.
* [**Lima AI agents**](https://lima-vm.io/docs/examples/ai/): Official Lima docs for running AI agents (Aider, Claude Code, Codex, Gemini) in isolated VMs with mount-only access to the project directory.
* [**Using Lima and Bash dotfiles to go fast with Claude Code**](https://blog.carlosnunez.me/post/using-lima-and-bash-dotfiles-to-go-fast-with-claude-code/): Practical setup for running Claude Code inside Lima VMs with dotfiles integration.
* [**APERTVS.ai**](https://apertvs.ai/) / [**swiss-ai/pretrain-data**](https://github.com/swiss-ai/pretrain-data): Apertus, a fully open foundation model for sovereign AI from the Swiss AI initiative — includes pretraining data reconstruction scripts.
* [**LocalAI**](https://localai.io/): Free, OpenAI/Anthropic-compatible all-in-one local inference stack.
* [**Linux kernel's 'second-in-command' uses local AI bot to hunt bugs**](https://www.tomshardware.com/software/linux/linux-kernels-second-in-command-uses-framework-desktop-to-hunt-bugs-with-local-ai) / [**The New Linux Kernel AI Bot**](https://www.phoronix.com/news/Clanker-T1000-AMD-Ryzen-AI-Max): Greg Kroah-Hartman's "Clanker T1000" — a local LLM fuzzing and bug-hunting system running on a Framework Desktop with AMD Ryzen AI Max+, resulting in close to two dozen kernel patches.
* [**Where the goblins came from**](https://openai.com/index/where-the-goblins-came-from/): OpenAI post-mortem on how personality-driven "goblin" outputs spread in GPT-5 — timeline, root cause, and fixes.
* [**Running Local LLMs Offline on a Ten-Hour Flight**](https://deploy.live/blog/running-local-llms-offline-on-a-ten-hour-flight/): Testing Gemma 4 31B and Qwen 4.6 36B via LM Studio on a MacBook Pro M5 Max (128GB) on a London-to-Vegas flight with no Wi-Fi.
* [**MLX**](https://ml-explore.github.io/mlx/build/html/index.html) / [**ml-explore/mlx**](https://github.com/ml-explore/mlx): Apple's MLX — an array framework for machine learning on Apple Silicon.
* [**How I Measured 1 Tonne of CO2 from My AI Coding Sessions**](https://dev.to/gwittebolle/how-i-measured-1-tonne-of-co2-from-my-ai-coding-sessions-3b3d): Measuring the environmental footprint of AI-assisted development.
* [**Taalas — The model is The Computer**](https://taalas.com/) / [**chat jimmy**](https://chatjimmy.ai/): Taalas turns deep learning models into custom silicon — chat jimmy is their LLM web interface, capable of 25k tokens/s inference.
* [**sci-bot**](https://sci-bot.ru/): AI-powered research assistant.

## Claude Code & AI Coding Tools

* [**Orchestrate teams of Claude Code sessions**](https://code.claude.com/docs/en/agent-teams): Official Claude Code docs for coordinating multiple instances with shared tasks, inter-agent messaging, and centralized management.
* [**Manage costs effectively**](https://code.claude.com/docs/en/costs#settings-json): Claude Code cost management — token usage tracking, spend limits, context management, model selection, and preprocessing hooks.
* [**Common workflows**](https://code.claude.com/docs/en/common-workflows#run-parallel-claude-code-sessions-with-git-worktrees): Claude Code guide including parallel sessions with git worktrees.
* [**Conductor**](https://www.conductor.build/): Mac app for running parallel Codex + Claude Code agents in isolated workspaces — see what they're working on at a glance, then review and merge.
* [**endorhq/flightplanner**](https://github.com/endorhq/flightplanner): Framework-agnostic E2E testing principles and AI-assisted workflows for coding agents.
* [**ralph-wiggum**](https://looking4offswitch.github.io/blog/2026/01/04/ralph-wiggum-claude-code/): Claude Code plugin for autonomous, long-running multi-task execution loops.
* [**Claude Code On-The-Go**](https://granda.org/en/2026/01/02/claude-code-on-the-go/): Running six Claude Code agents in parallel from an iPhone via cloud VM, Tailscale, mosh, and push notifications.
* [**Plugins for Claude Code**](https://claude.com/plugins) / [**CLAUDE.md Management plugin**](https://claude.com/plugins/claude-md-management): Claude Code plugin marketplace — including a plugin to maintain and audit CLAUDE.md files.
* [**openclaw/clawsweeper**](https://github.com/openclaw/clawsweeper) / [**openclaw/clownfish**](https://github.com/openclaw/clownfish) / [**openclaw/gitcrawl**](https://github.com/openclaw/gitcrawl): Steipete's AI-powered GitHub maintenance stack — ClawSweeper scans issues/PRs weekly to suggest closures, Clownfish resolves issue clusters at scale, gitcrawl crawls for maintainer triage. [Closed ~4000 issues in a single day](https://x.com/steipete/status/2047982647264059734).
* [**nilbuild/diffity**](https://github.com/nilbuild/diffity): GitHub-style diff viewer for reviewing code changes from Claude Code, Cursor, and other AI tools.
* [**Vibe Maintainer**](https://steve-yegge.medium.com/vibe-maintainer-a2273a841040): Steve Yegge on what it's like maintaining a large OSS project flooded with AI-generated PRs.
* [**How I use AI in 2026**](https://fedepaol.github.io/blog/2026/04/25/how-i-use-ai-in-2026/): A maintainer and developer's practical AI workflow — coding, triaging PRs, and handling CI failures.
* [**systalyze/utilyze**](https://github.com/systalyze/utilyze) / [**Systalyze**](https://www.systalyze.com/utilyze): Platform for uncovering and eliminating inefficiencies in AI workloads — claims up to 90% cost reduction.

## Linux & Systems

* [**Progress Report: Linux 7.0 — Asahi Linux**](https://asahilinux.org/2026/04/progress-report-7-0/): Asahi Linux progress report tracking Linux 7.0 support for Apple Silicon.
* [**Project:Asahi/Guide — Gentoo Wiki**](https://wiki.gentoo.org/wiki/Project:Asahi/Guide): Guide to running Linux on Apple Silicon via Gentoo.
* [**Ubuntu 26.04 can install APT packages from GitHub Container Registry**](https://medium.com/nttlabs/ubuntu-26-04-can-install-apt-packages-from-github-container-registry-532412990318): Ubuntu 26.04 ships with support for installing APT packages hosted on OCI-compliant registries like GHCR.
* [**ps5-linux released**](https://x.com/theflow0/status/2049255768428347566) / [**ps5-linux/ps5-linux-loader**](https://github.com/ps5-linux/ps5-linux-loader): PS5 Phat (3.xx and 4.xx firmware) can now boot Linux as a fully functional PC gaming device via HV exploit and custom bootloader.
* [**HardenedBSD Officially on Radicle**](https://hardenedbsd.org/article/shawn-webb/2026-04-26/hardenedbsd-officially-radicle) / [**Radicle**](https://radicle.dev/): HardenedBSD moves to Radicle, the peer-to-peer sovereign code forge built on Git.
* [**Managing Secrets In Linux**](https://grahamwatts.co.uk/gnome-secrets/): Tools and approaches for secrets management on Linux, covering GNOME Keyring and alternatives.

## Development, Web & Tools

* [**Ghostty Is Leaving GitHub**](https://mitchellh.com/writing/ghostty-leaving-github): Mitchell Hashimoto explains why the Ghostty terminal emulator is moving away from GitHub.
* [**con**](https://con.nowledge.co/): Open-source, GPU-accelerated terminal with a built-in AI harness for SSH, tmux, and agent-native workflows.
* [**foot — ArchWiki**](https://wiki.archlinux.org/title/Foot): ArchWiki page for foot, a fast, lightweight Wayland terminal emulator.
* [**Quarkdown**](https://quarkdown.com/): Modern open-source Markdown-based typesetting system for papers, presentations, knowledge bases, and static sites.
* [**Managing Secrets In macOS**](https://grahamwatts.co.uk/macos-secrets/): Tools for secrets management on macOS — companion to the Linux article above.
* [**interblah.net — Self-updating screenshots**](https://interblah.net/self-updating-screenshots): A technique for keeping screenshots in documentation automatically up to date.
* [**From Milliseconds to 26 Nanoseconds: How a $20 eBay SFP Module Beat My Entire NTP Setup**](https://austinsnerdythings.com/2026/04/26/ptp-osa5401-26-nanoseconds-raspberry-pi/): Using a cheap SFP module and PTP on a Raspberry Pi to achieve 26ns time accuracy — dramatically better than GPS-based NTP.

## Apple / macOS

* [**How fast is a macOS VM, and how small could it be?**](https://eclecticlight.co/2026/05/02/how-fast-is-a-macos-vm-and-how-small-could-it-be/): Geekbench performance figures for macOS VMs and testing the minimum cores/memory needed to run one usably on a MacBook.
* [**Networking changes coming in macOS 27**](https://eclecticlight.co/2026/04/23/networking-changes-coming-in-macos-27/): AFP removal and new server connection requirements coming in macOS 27 — what it means for your setup.
* [**Apple wants to kill your Time Capsule, but they run NetBSD so they can't**](https://www.osnews.com/story/144845/apple-wants-to-kill-your-time-capsule-but-they-run-netbsd-so-they-cant/) / [**jamesyc/TimeCapsuleSMB**](https://github.com/jamesyc/TimeCapsuleSMB): Time Capsules run NetBSD, which complicates Apple's ability to remote-kill them. TimeCapsuleSMB hacks the device to run modern Samba.
* [**x56/airpyrt-tools**](https://github.com/x56/airpyrt-tools) / [**noname122021/airpyrt-tools-guide**](https://github.com/noname122021/airpyrt-tools-guide): Python client and guide for unlocking AirPort Extreme (A1521) on Apple Silicon — enable SSH, remove region limits (FCC boost), and control hardware fans.

## Fun & Misc

* [**synth.html v0.7.0**](https://zpeters.github.io/synth-html/): A modular synthesizer in a single HTML file — no server, no build step, no npm install. Drag nodes, patch cables, and sculpt sound like it's 1972 but your browser is the Moog.
* [**Is my blue your blue?**](https://ismy.blue/): Interactive color perception test — does everyone see the same blue?
* [**¿Cuánto te cuestan realmente tus gastos?**](https://rentabilidadreal.com/calculadora-coste-oportunidad/?esc%3Dcafe%26rent%3D7%26inf%3D2.5%26precioUnidad%3D2%26frecuencia%3D2%26anos%3D20): Opportunity cost calculator (in Spanish) — what your daily coffee actually costs in 20 years at a 7% return.
