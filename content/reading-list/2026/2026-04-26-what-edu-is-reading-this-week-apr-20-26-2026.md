---
title: "What Edu is reading this week (April 20 - 26, 2026)"
date: 2026-04-25T10:00:00+02:00
draft: false
slug: 2026-04-26-what-edu-is-reading-this-week-apr-20-26-2026
aliases:
  - /posts/2026-04-26-what-edu-is-reading-this-week-apr-20-26-2026/
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
---

This week features a heavy focus on AI agent tooling and Claude Code in particular, a notable cluster of sandboxing and security links, fresh SDR and hardware hacking projects, and a few significant industry moments including Apple's leadership change and Intel pulling back from open source.

![Reading list header image](/images/2026-04-26-what-edu-is-reading-this-week-apr-20-26.png)

## Cloud, Kubernetes & Infrastructure

* [**Btrfs | Internals for Interns**](https://internals-for-interns.com/posts/btrfs-filesystem/) - A deep dive into Btrfs internals, exploring how its copy-on-write design sets it apart from filesystems like ext4 and XFS that modify data in place.
* [**harche/nemoclaw-operator**](https://github.com/harche/nemoclaw-operator) - A Kubernetes operator for deploying NemoClaw on OpenShift.
* [**Hidden Infrastructure Challenges in Distributed LLM Inference on Kubernetes**](https://substack.com/home/post/p-188586336) - A networking-focused look at the infrastructure complexity of running distributed LLM inference workloads on Kubernetes.
* [**Community Blueprints Repo: Common self-hosted apps exposed with Pangolin via Docker labels**](https://www.reddit.com/r/PangolinReverseProxy/comments/1sr03g6/community_blueprints_repo_common_selfhosted_apps/) - A community repo making it easy to expose common self-hosted apps like Grafana, Immich, and Nextcloud through Pangolin using Docker labels.

## AI, Agents & Tools

* [**no1msd/seance**](https://github.com/no1msd/seance) - A scrolling terminal multiplexer designed specifically for tracking multiple AI coding agents simultaneously.
* [**How LLMs Work — A Visual Deep Dive**](https://ynarwal.github.io/how-llms-work/) - An interactive visual guide explaining the internals of large language models.
* [**Vibe coding (Andrej Karpathy)**](https://x.com/karpathy/status/1886192184808149383) - Karpathy's original post coining "vibe coding" — fully giving in to LLM-driven development and letting go of reading the code.
* [**Introducing GPT-5.5**](https://openai.com/index/introducing-gpt-5-5/) - OpenAI's announcement of GPT-5.5, targeted at complex coding, research, and data analysis tasks across tools.
* [**An update on recent Claude Code quality reports**](https://www.anthropic.com/engineering/april-23-postmortem) - Anthropic's engineering postmortem addressing reported quality regressions in Claude Code.
* [**Anthropic and Amazon expand collaboration for up to 5 gigawatts of new compute**](https://www.anthropic.com/news/anthropic-amazon-compute) - Anthropic and Amazon's announcement of an expanded partnership covering significant new compute infrastructure.
* [**Anthropic secretly installs spyware when you install Claude Desktop**](https://www.thatprivacyguy.com/blog/anthropic-spyware/) - A privacy researcher's claim that Claude Desktop silently installs a Native Messaging bridge into multiple Chromium browsers, including unsupported ones.
* [**The Agentic SDLC Handbook**](https://danielmeppiel.github.io/agentic-sdlc-handbook/) - A handbook covering the software development lifecycle adapted for AI agent workflows.
* [**val4oss/ai-agents-sandbox**](https://github.com/val4oss/ai-agents-sandbox) - A secure, isolated container environment for running AI coding agents.
* [**DESIGN.md open-source spec**](https://x.com/i/status/2046624729403142320) - Open-sourcing of the DESIGN.md specification, which lets agents import and export design rules across projects and tools instead of guessing intent.
* [**code-yeongyu/oh-my-openagent**](https://github.com/code-yeongyu/oh-my-openagent) - An agent harness previously known as oh-my-opencode, aiming to be the best CLI agent framework.
* [**Skill Authoring Patterns from Anthropic's Best Practices**](https://generativeprogrammer.com/p/skill-authoring-patterns-from-anthropics) - A breakdown of recurring design patterns for building effective Claude Skills, covering activation metadata and executable helpers.
* [**cmux — The terminal built for multitasking**](https://cmux.com/) - A native macOS terminal designed for running multiple AI coding agents simultaneously, compatible with Claude Code, Codex, Gemini CLI, and more.
* [**How Claude Code works**](https://code.claude.com/docs/en/how-claude-code-works) / [**Explore the context window**](https://code.claude.com/docs/en/context-window) / [**Customize your status line**](https://code.claude.com/docs/en/statusline): A trio of official Claude Code docs covering the agentic loop, an interactive context window cost simulation, and custom status bar configuration.
* [**Writing a good CLAUDE.md**](https://www.humanlayer.dev/blog/writing-a-good-claude-md) / [**Best Practices for Claude Code**](https://code.claude.com/docs/en/best-practices#write-an-effective-claude-md): A community guide and official documentation on writing effective CLAUDE.md files and getting the most out of Claude Code.
* [**The complete Claude Code tutorial**](https://x.com/eyad_khrais/status/2010076957938188661?s=46&t=80WYPk2R5ciaENgyFZn_fA) - A comprehensive Claude Code tutorial thread.
* [**Home - Crawl4AI Documentation**](https://docs.crawl4ai.com/) - Docs for Crawl4AI, an open-source LLM-friendly web crawler and scraper.
* [**Best Ollama Models for Coding in 2026**](https://www.aimadetools.com/blog/best-ollama-models-coding-2026/) - A benchmark of ten local coding models running in Ollama, including Devstral, Qwen 3.6, DeepSeek, and Codestral.
* [**I Benchmarked the Viral "Caveman" Prompt to Save LLM Tokens**](https://medium.com/@KubaGuzik/i-benchmarked-the-viral-caveman-prompt-to-save-llm-tokens-then-my-6-line-version-beat-it-d8e565f95e15) - Testing the caveman token-reduction prompt versus a simpler 6-line version, with the latter coming out ahead.

## Sandboxing & Security

* [**Source code sandboxing**](https://kristaps.bsd.lv/devsecflops/) / [**HN Discussion**](https://news.ycombinator.com/item?id=44249511): An exploration of sandboxing techniques for securing development environments and the accompanying Hacker News discussion.
* [**Quick 'n Dirty seatbelt/sandbox**](https://gist.github.com/n8henrie/eaaa1a25753fadbd7715e85a38b99831) - A minimal macOS seatbelt sandbox profile for quick process isolation.
* [**Landlock LSM: kernel documentation**](https://docs.kernel.org/security/landlock.html) - Official Linux kernel documentation on Landlock, the unprivileged access control LSM.
* [**OSX Sandboxing Design**](https://www.chromium.org/developers/design-documents/sandbox/osx-sandboxing-design/) - Chromium's documentation on the macOS sandboxing design used to isolate renderer processes.
* [**bindsch/scode**](https://github.com/bindsch/scode) - A safe sandbox wrapper for AI coding harnesses.
* [**Sandboxing - Claude Code Docs**](https://code.claude.com/docs/en/sandboxing) / [**Sandboxing Claude Code with nono**](https://nono.sh/docs/cli/clients/claude-code): Official Claude Code documentation on the sandboxed bash tool for filesystem and network isolation, alongside a guide for using nono as the sandboxing backend.
* [**Bitwarden CLI Compromised in Ongoing Checkmarx Supply Chain Attack**](https://socket.dev/blog/bitwarden-cli-compromised) - Report on Bitwarden CLI 2026.4.0 being compromised via GitHub Action abuse in Bitwarden's CI/CD pipeline.

## Linux & Systems

* [**Ubuntu 26.04 LTS release notes**](https://documentation.ubuntu.com/release-notes/26.04/) - Release notes for Ubuntu 26.04 LTS (Resolute Raccoon) covering new features and changes.
* [**Git worktree like a boss**](https://dev.to/metal3d/git-worktree-like-a-boss-2j1b) - A practical guide to Git's worktree feature, one of the most underused tools in everyday Git workflows.

## SDR, Hardware & Electronics

* [**BrowSDR**](https://github.com/jLynx/BrowSDR) / [**RTL-SDR.com article**](https://www.rtl-sdr.com/browsdr-turn-your-hackrf-or-rtl-sdr-into-a-browser-based-remote-websdr/): An open-source browser-based SDR receiver connecting via WebUSB with a Rust/WASM DSP pipeline, supporting WFM, NFM, AM, SSB, CW, raw IQ, RDS, and POCSAG.
* [**Lucaslhm/Flipper-IRDB**](https://github.com/Lucaslhm/Flipper-IRDB) / [**Zero-Sploit/FlipperZero-Subghz-DB**](https://github.com/Zero-Sploit/FlipperZero-Subghz-DB/tree/main/subghz) / [**i12bp8/TagTinker**](https://github.com/i12bp8/TagTinker): Community signal databases and apps for the Flipper Zero, covering IR codes, sub-GHz captures, and electronic shelf label (ESL) research.
* [**Bruce Firmware**](https://bruce.computer/) - A predatory ESP32 firmware project for security research and RF/hardware hacking.
* [**OctoPrint 2.0.0 is coming soon!**](https://octoprint.org/blog/2026/04/20/octoprint-2.0.0-is-coming-soon/) - Announcement of OctoPrint 2.0.0's first release candidate, covering breaking changes and plugin compatibility.
* [**Tech1k/helloesp**](https://github.com/Tech1k/helloesp) / [**helloesp.com**](https://helloesp.com/): A fully functional public website hosted on an ESP32 microcontroller with 520 KB of RAM.

## Development & Tools

* [**Laws of Software Engineering**](https://lawsofsoftwareengineering.com/) - A collection of principles and patterns shaping software systems, teams, and decisions.
* [**TomBadash/Mouser**](https://github.com/TomBadash/Mouser) - A lightweight, open-source, fully local alternative to Logitech Options+ for remapping Logitech HID++ mice.

## Fun & Misc

* [**Meshcore.io - Why The Split?**](https://blog.meshcore.io/2026/04/23/the-split) - MeshCore's explanation of their migration to a new site and organizational split.
* [**Fusion Power Plant Simulator**](https://www.fusionenergybase.com/fusion-power-plant-simulator) - An interactive diagram for exploring energy flows in a fusion power plant by adjusting Q values and efficiencies.
* [**Tim Cook to become Apple Executive Chairman; John Ternus to become Apple CEO**](https://www.apple.com/newsroom/2026/04/tim-cook-to-become-apple-executive-chairman-john-ternus-to-become-apple-ceo/) / [**Tim Cook's Impeccable Timing**](https://stratechery.com/2026/tim-cooks-impeccable-timing/): Apple's official leadership transition announcement alongside Ben Thompson's analysis of Cook's tenure and the timing of his exit.
* [**Intel shutters open-source evangelism program**](https://www.tomshardware.com/software/intel-shutters-open-source-evangelism-program-and-archives-key-community-projects-closures-point-to-significant-shift-in-open-source-leadership) - Intel archiving key community open-source projects amid ongoing restructuring, pointing to a significant shift in its open-source leadership.
* [**Vietnam Mario Kart theme park**](https://x.com/reizisokk/status/2047271429050433900) - A viral post about a Mario Kart-style theme park in Vietnam.
* [**A hairdryer broke Polymarket's Paris weather markets**](https://x.com/aaronjmars/status/2047017251270734309) - The story of someone gaming Polymarket's Paris temperature predictions by placing a hairdryer near an unguarded Météo France sensor at CDG airport, netting $34,000.
