---
title: "What Edu is reading this week (Sep 19 - 26, 2026)"
date: 2026-09-26T09:00:00+02:00
draft: false
slug: 2026-09-26-what-edu-is-reading-this-week-sep-19-26-2026
aliases:
  - /posts/2026-09-26-what-edu-is-reading-this-week-sep-19-26-2026/
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
  - agents
  - android
  - networking
  - homelab
  - hardware
---

Two frontier model releases shared the week with a widening set of small decision models and agent runtimes, and with more reports on how coding agents are changing day-to-day development. On the infrastructure side: kernel live-update work to keep VMs running, DRBD releases, router and Android tooling, and a Playdate app for watching live air traffic.

## AI, Agents & Models

* [**Introducing GPT-6 Sol and Luna**](https://openai.com/index/introducing-gpt-6-sol-and-luna/) - OpenAI's two new models, aimed at everyday work with different balances of capability and cost.
* [**Introducing Claude Opus 5.5**](https://www.anthropic.com/claude-opus-5-5) - Anthropic's new flagship for agentic coding and knowledge work, which the announcement says costs about 40% less to run than Opus 5 on typical workloads.
* [**google/ax**](https://github.com/google/ax) / [**AX**](https://agentexecutor.io/) - Google's open agentic orchestration runtime: declare a task in YAML, and AX sandboxes it, wires up the workspace, fences the network and runs many of them per cluster.
* [**hermes-jev-skills**](https://github.com/kerpopule/hermes-jev-skills) - Moves the small decisions (which model answers a turn, which skills to load, which retrieved passages matter) off the frontier model and onto a cheap classifier, for Hermes agents as well as Claude Code and Codex.
* [**Welcome back to Hermes Agent, Claude**](https://x.com/Teknium/status/2102093483788107792) - Teknium on the new official plugin that wraps the Claude SDK, so Claude Code subscriptions work in Hermes Agent again.
* [**I asked Meta's Muse for its filesystem and it sent me 6.8 GB**](https://mouse.dev/blog/muse-runtime-export/) - What happens when you ask an agent to archive everything it can see and send it to your Drive: it does, and the write-up looks at what that says about agent runtimes.
* [**Claude Code reads AGENTS.md only when telemetry is on**](https://blog.szypowi.cz/p/claude-code-reads-agents.md-only-when-telemetry-is-on/) - Measurements showing AGENTS.md support sits behind a remote feature flag, so a local AGENTS.md is skipped without warning when telemetry or nonessential traffic is off, plus the one-line CLAUDE.md workaround.

## Decision Models & Small Runtimes

* [**JevBench v1.2**](https://benchmarkheaven.com/jev-models) - Scores Jev, its open rebuilds and instruction models on intelligence, calibration, speed and cost, 25% each.
* [**featherless-ai/simple-jev**](https://github.com/featherless-ai/simple-jev) / [**Simple Jev**](https://simple-jev.featherless.ai/) - An open source implementation of Jev that turns any open model into a classifier endpoint, with a demo API you can call without a key.
* [**jaredpalmer/kev**](https://github.com/jaredpalmer/kev) - Small Jev-like decision models built on Qwen3.5 and Qwen3.8, with pretrained weights or a training run of your own.
* [**mizorewww/laya-mlx**](https://github.com/mizorewww/laya-mlx) - A native MLX runtime for Laya typed decision models, reporting 7-14 ms short decisions on an M3 Max without text generation or a cloud API.

## Learning & Self-Teaching

* [**Magic for self-learners**](https://www.reddit.com/r/hermesagent/comments/1wpe0wv/magic_for_selflearners/) - A r/hermesagent thread on how the latest models changed the way the author learns things, after years of using them badly.
* [**madhvantyagi/Gnos**](https://github.com/madhvantyagi/Gnos) - A teaching harness that turns a coding agent into a teacher: it designs a curriculum, generates videos, simulations, images and PDFs, and tracks your learning style. Ships as Codex and Claude Code plugins under the MIT license.

## Cloud, Kubernetes & Infrastructure

* [**Orphaned VMs: running VMs uninterrupted while the host kernel is offline**](https://www.phoronix.com/news/Orphaned-VMs-Linux-Patches) - RFC patches that keep guests executing on preserved physical CPUs across a host kernel live update, using the Live Update Orchestrator. Tested on Intel, AMD and Arm, and still very early work.
* [**nestrilabs/virtio-nvgpu**](https://github.com/nestrilabs/virtio-nvgpu) - An experimental virtio device for near-native NVIDIA GPU access inside KVM virtual machines.
* [**drbd-9.2.20 and drbd-9.3.4**](https://forums.linbit.com/t/drbd-9-2-20-and-drbd-9-3-4/1275) - LINBIT's release notes, with a note on how a year of Claude Code use let the team fit more fixes into a cycle than ever: reproducers, DRBD-specific static analyzers, a deterministic simulator. The 9.2.x series is nearly done.

## Linux, Routers & Homelab

* [**Abandoning Scientific Linux Was a Mistake**](https://blog.melashri.net/posts/scientific-linux-mistake/) - On CERN moving its accelerator front-end systems to Debian 13, and why the scientific community running its own distribution was worth the effort even while CentOS was around.
* [**kobidarch/luci-theme-doodle**](https://github.com/kobidarch/luci-theme-doodle) - A pastel doodle theme for the OpenWrt LuCI web interface: paper cards, 3px ink borders, hard offset shadows. Light mode only for now.
* [**686f6c61/DIGI-F8748**](https://github.com/686f6c61/DIGI-F8748) - Recovers the admin password of a DIGI ZTE F8748 router without installing anything and without touching the existing configuration, step by step, with scripts for macOS, Linux and Windows.
* [**CidVonHighwind/pocketfin**](https://github.com/CidVonHighwind/pocketfin) - A Jellyfin client for the PlayStation Portable: movies and shows from your own server on a Memory Stick console over the PSP's 2.4 GHz Wi-Fi.

## Security & Privacy

* [**Containers Are No Longer a Security Boundary**](https://depthfirst.com/research/containers-are-no-longer-safe) - A walk through CVE-2026-80521, an AF_UNIX use-after-free found with an in-house AI vulnerability model, and the argument that sensitive or untrusted workloads belong in Firecracker or Kata Containers.
* [**I said no and Apple said yes**](https://dbushell.com/2026/09/22/apple-intelligence/) - David Bushell on Apple Intelligence, and on what a consent prompt is worth when the answer is treated as yes anyway.

## Development, Web & Design

* [**AI-generated posters don't have to be horrible**](https://john.hartnup.uk/2026/06/07/ai-event-posters.html) - Why AI event posters end up looking interchangeable, and how naming a specific design style and era, from Bauhaus to punk fanzine, gets usable results.
* [**Bastardica**](https://bastardica.mitpit.com) - A browser tool and type foundry for "bastard" fonts: mix glyphs from several fonts through a liga substitution, tune stride and effects, and export TTF, OTF or WOFF2. Everything runs locally with Pyodide.

## Android & Mobile

* [**F-Droid 2.0**](https://f-droid.org/2026/09/24/f-droid-2.0-a-new-chapter-for-android-freedom.html) - The app's largest update in ten years: a Material-based redesign rewritten in Kotlin Compose, better search and discovery, rolling out over the coming weeks. The post also points to the keepandroidopen.org campaign about Google's installer changes.
* [**tgeorgiadis/quiver-launcher**](https://github.com/tgeorgiadis/quiver-launcher) - An Android and desktop launcher for apps distributed through GitHub and GitLab releases, with a personal library, subscribable community catalogs and filtering.

## Hardware & Smart Home

* [**Shelly Group / Schneider Electric takeover**](https://corporate.shelly.com/en/news/shelly-group-has-entered-into-an-investment-agreement-with-schneider-electric-on-the-intended-voluntary-public-takeover) - Schneider Electric intends to offer EUR 70 per share for Shelly Group, roughly EUR 1.2 billion and a 27% premium, with both founders supporting the deal; closing is expected by Q1 2027.
* [**Porsche puts wireless EV charging into production**](https://electrek.co/2026/09/18/its-finally-here-porsche-puts-wireless-ev-charging-into-production-video/) - Wireless Charging arrives on the Cayenne Electric: park over a ground pad and charge at up to 11 kW and about 90% efficiency, with motion and foreign-object detection that stops the process when a living creature comes close.

## Fun & Off-Topic

* [**Flight Radar by Darkerbulb**](https://darkerbulb.itch.io/flight-radar) - Turns a Playdate into a live air-traffic scope: real ADS-B traffic on a sonar-style display, selectable ranges, per-flight details and real ATC audio for the selected flight. It is being rebuilt right now after an ATC audio bug.
* [**No Sloptober**](https://no-sloptober.com/) - An October challenge to go without LLM-based tools entirely, as a way to rebuild your own sense of what they are good and bad at. The hard mode turns off AI search summaries and code review too, not just chat.
