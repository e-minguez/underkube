---
title: "What Edu is reading this week (May 24 - 30, 2026)"
date: 2026-05-30T10:00:00+02:00
draft: false
slug: 2026-05-30-what-edu-is-reading-this-week-may-24-30-2026
aliases:
  - /posts/2026-05-30-what-edu-is-reading-this-week-may-24-30-2026/
categories:
  - Reading
tags:
  - newsletter
  - links
  - tech
  - devops
  - linux
  - ai
  - hardware
  - networking
---

Claude Opus 4.8 dropped and the Claude Code ecosystem exploded this week — undocumented configs, deep-dive guides, GitHub Actions, and tools to catch the slop agents leave behind. Also: Gentoo speedruns, Linux Secure Boot expiration concerns, mesh networking deep-dives, and ambient sound apps.

![What Edu is reading this week (May 24 - 30, 2026)](/images/2026-05-30-what-edu-is-reading-this-week-may-24-30.png)

## AI, Agents & Tools

* [**Introducing Claude Opus 4.8**](https://www.anthropic.com/news/claude-opus-4-8): Anthropic's latest Opus-class upgrade — stronger coding, better agentic task handling, and improved consistency for long-running work.
* [**I think Anthropic and OpenAI have found product-market fit**](https://simonwillison.net/2026/May/27/product-market-fit/): Simon Willison on Anthropic's first rumored profitable quarter and the growing surprise of how expensive LLM bills are becoming from real usage.
* [**I Read the Claude Code Source Code. Here's Everything You Can Configure That the Docs Don't Tell You.**](https://buildingbetter.tech/p/i-read-the-claude-code-source-code): Hook fields that rewrite commands mid-flight, persistent agent memory, auto-mode rules in plain English, and self-improving loops — all undocumented, all copy-paste ready.
* [**Beyond the Prompt: Claude Code**](https://arps18.github.io/posts/claude-code-mastery/): Deep dive into the `.claude` directory, CLAUDE.md, skills, custom subagents, plugins, and underused commands like `/goal` and `/insights`. Covers the workflow patterns the Anthropic team actually uses.
* [**mattpocock/skills**](https://github.com/mattpocock/skills): Matt Pocock's Claude Code skills library — real, opinionated skills straight from his `.claude` directory.
* [**anthropics/claude-code-action**](https://github.com/anthropics/claude-code-action): Official GitHub Action for running Claude Code in CI — useful for automated code review and agentic PR workflows.
* [**scanaislop/aislop**](https://github.com/scanaislop/aislop): Deterministic, sub-second linter that catches the slop AI coding agents leave in your code — 40+ rules across 7 languages, no LLM needed. MIT.
* [**srbarrios/agentic-test-explorer**](https://github.com/srbarrios/agentic-test-explorer): AI-driven exploratory test framework — intelligently explores, tests, and validates any application. Language-agnostic.
* [**teng-lin/notebooklm-py**](https://github.com/teng-lin/notebooklm-py): Unofficial Python API and agentic skill for Google NotebookLM — full programmatic access including features the web UI doesn't expose, plus CLI support.
* [**Using AI to write better code more slowly**](https://nolanlawson.com/2026/05/25/using-ai-to-write-better-code-more-slowly/): A pushback on the "AI = fast slop" narrative — making the case for using AI as a deliberate, quality-focused tool rather than a code-spewing machine.
* [**The Trick Behind the AI Magic: Explain AI to Your Manager in Plain English**](https://hackernoon.com/the-trick-behind-the-ai-magic-explain-ai-to-your-manager-in-plain-english): The simple concept behind the magic, why it feels so powerful, and why it matters — a good coffee-break explainer for non-technical people.

## Linux & Systems

* [**Why Gentoo?**](https://blogs.gentoo.org/mgorny/2026/05/28/why-gentoo/): Michał Górny breaks down what makes Gentoo different beyond the compiling stereotype — the philosophy, flexibility, and the kind of user it's actually built for.
* [**GENTOO SPEEDRUN - 1:34**](https://www.youtube.com/watch?v=PGhTedqoKMA): Full Gentoo install in 1 minute 34 seconds on a KVM VM with a custom DNS trick to cache distfiles on the host. Impressively fast.
* [**Linux and Secure Boot certificate expiration**](https://lwn.net/Articles/1029767/) / [**Microsoft secure boot certificate changes**](https://support.scc.suse.com/s/kb/Microsoft-secure-boot-certificate-changes?language=en_US): A Microsoft Secure Boot signing certificate used by most Linux distros is expiring — if you have Secure Boot enabled, this may affect your system. LWN has the background; SUSE has the mitigation steps.
* [**Flatpak will depend on systemd**](https://www.osnews.com/story/145071/flatpak-will-depend-on-systemd/): OSnews covers Flatpak's move to require systemd — predictably contentious for non-systemd distros.
* [**your_dotfiles_are_not_a_distro**](https://abyss.fish/your_dotfiles_are_not_a_distro): Short, punchy take on the dotfiles-as-identity problem. Worth a read if you've ever been tempted to call your config a "distribution".

## Networking, Smart Home & Hardware

* [**I'm Getting Into Mesh Networks... (Meshtastic, MeshCore, and Reticulum)**](https://www.jonaharagon.com/posts/im-getting-into-mesh-networks-meshtastic-meshcore-and-reticulum/): Jonah Aragon — who runs their own ISP with an ASN and fiber — goes deeper into decentralized mesh networking. Good practical overview of three different protocols.
* [**DynIP — Dynamic DNS that actually works**](https://dynip.dev/): 60-second updates, RFC 2136 TSIG, BYOD, DNSSEC — aimed at homelabs, edge routers, and infrastructure teams.
* [**These metal washers are replacing smart home sensors**](https://www.xda-developers.com/coin-sized-sensors-could-eliminate-smart-home-batteries-forever/): Coin-sized passive sensors with no batteries and no wires — potentially a significant shift for home automation.
* [**strepto42/homeassistant-esptimecast**](https://github.com/strepto42/homeassistant-esptimecast): HACS-compatible Home Assistant integration for esptimecast.

## Development & Tools

* [**The pressure**](https://daniel.haxx.se/blog/2026/05/26/the-pressure/): Daniel Stenberg (curl author) on the real pressures of open source maintenance — social, financial, and emotional. Important reading.
* [**gollum/gollum**](https://github.com/gollum/gollum): Simple, Git-powered wiki with a local web frontend and support for many markup formats. Good for personal or team knowledge management.
* [**Mini Micro**](https://miniscript.org/MiniMicro/index.html#about): A fantasy microcomputer — retro-style computing environment with a modern scripting language. Fun for programming experimentation and learning.
* [**A few interesting modern pixel fonts**](https://unsung.aresluna.org/a-few-interesting-modern-pixel-fonts/): A curated look at pixel fonts worth actually using — not just retro nostalgia, but genuinely useful typefaces.

## Sound & Ambient

* [**rafaelmardojai/blanket**](https://github.com/rafaelmardojai/blanket) / [**codybrom/Blankie**](https://github.com/codybrom/Blankie) / [**elytraVIII/ElytAmbience**](https://github.com/elytraVIII/ElytAmbience): Three ambient sound apps for three platforms — Blanket for GNOME, Blankie for macOS (App Store + Homebrew), and ElytAmbience for BSD desktops (FreeBSD/GhostBSD) — a high-performance native rewrite of Blanket.

## Fun & Misc

* [**Ten Basic Clouds**](https://www.noaa.gov/jetstream/clouds/ten-basic-clouds): NOAA's guide to the ten basic cloud types — a surprisingly pleasant rabbit hole into cloud classification and meteorology.
* [**It's hard to justify Tahoe icons**](https://tonsky.me/blog/tahoe-icons/): Niki Tonsky dissects Apple's icon redesign in macOS Tahoe against first principles — and finds them wanting.
* [**taigrr/spank**](https://github.com/taigrr/spank): Slap your MacBook, it yells back. Uses the Apple Silicon accelerometer via IOKit HID. MIT.
* [**Ferrari Luce**](https://www.ferrari.com/en-EN/auto/ferrari-luce): A first look at the Ferrari Luce interior and interface — not tech, but beautifully engineered.
* [**pa k kieres tener cocina jaja saludos**](https://pelusococina.substack.com/p/pa-k-kieres-tener-cocina-jaja-saludos): Peluso Cocina on what we sacrifice for convenience culture — in Spanish, worth reading.
