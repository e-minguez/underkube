---
title: "What Edu is reading this week (Sep 12 - 19, 2026)"
date: 2026-09-19T09:00:00+02:00
draft: false
slug: 2026-09-19-what-edu-is-reading-this-week-sep-12-19-2026
aliases:
  - /posts/2026-09-19-what-edu-is-reading-this-week-sep-12-19-2026/
categories:
  - Reading
tags:
  - newsletter
  - links
  - tech
  - devops
  - security
  - linux
  - bsd
  - ai
  - agents
  - kubernetes
  - storage
  - hardware
  - homelab
  - audio
  - gaming
---

Agent infrastructure dominated the week: Kubernetes-native harnesses, a high-density sandbox runtime on GKE, and a 27B model compressed into under 6 GB. Alongside that, BSD filesystem work, PipeWire audio tooling and a batch of retro-gaming archives.

## AI, Agents & Tools

* [**llmman**](https://github.com/llmmanorg/llmman) - Runs any agent on any model, with the models themselves stored and shipped as OCI images.
* [**Mecatl**](https://mecatl.dev/) - Stacklok's open source, cloud-native harness for agents: the agent loop, the sandbox and the state are separate components, so a fleet runs on Kubernetes instead of on your laptop.
* [**Agent Substrate available on GKE**](https://cloud.google.com/blog/products/containers-kubernetes/agent-substrate-available-on-gke) / [**agent-substrate/substrate**](https://github.com/agent-substrate/substrate) - Google's open source, high-density agent runtime, which it says scales to millions of sandboxes per cluster.
* [**Anthropic's Hidden Vercel Competitor "Antspace"**](https://aprilnea.me/en/blog/reverse-engineering-claude-code-antspace) - Reverse engineering the Claude Code client to find the deployment platform behind it.
* [**I Came, I Prompted, I Left Part 1**](https://codyho.dev/blog/hypervisor-macbook-neo/) - A custom hypervisor for the MacBook Neo, built to trace how macOS talks to Apple Silicon, mostly through unattended LLM loops.
* [**archify**](https://github.com/tt-a1i/archify) - An agent skill that turns a description into architecture, workflow and sequence diagrams as self-contained HTML, with dark/light themes and SVG/PNG export.
* [**PrismML: Bonsai 2 27B**](https://prismml.com/news/bonsai-2-27b) - A ternary-compressed 27B model that keeps 98.2% of Qwen3.8 27B's benchmark results in a 5.9 GB footprint.
* [**mimo-v2.6 RL**](https://mimo.xiaomi.com/rl/) - Live training metrics from the reinforcement learning runs behind Xiaomi's mimo-v2.6-pro and mimo-v2.6-flash.
* [**SemIf — local decisions in your browser**](https://openjev.com/) - Jev's System One model running locally on WebGPU, returning typed option logits and autoregressive JSON.
* [**awesome-jev**](https://github.com/kraayenjon/awesome-jev) / [**Made with Jev**](https://madewithjev.com/) - A curated list of Jev use cases, SDKs and resources, plus a directory of projects built with it and the cost and speed each author reported.
* [**mysetup.ai**](https://mysetup.ai/) - Publish your own AI setup and browse how other people run theirs.

## Cloud, Kubernetes & Storage

* [**When is a cluster really full?**](https://medium.com/@InditexTech/when-is-a-cluster-really-full-unlocking-hidden-capacity-with-the-k8s-overcommit-operator-9fd75af95712) / [**k8s-overcommit-operator**](https://github.com/InditexTech/k8s-overcommit-operator) - Inditex's operator for overcommitting pod resource requests, plus the write-up of how it halved microservice replicas through a 2025 demand peak.
* [**RustFS 1.0.0 GA**](https://rustfs.com/blog/announcing-rustfs-1-0-0-ga/) - An Apache-2.0, S3-compatible distributed object store written in Rust reaches general availability.

## Linux, BSD & Systems

* [**Crash-Safe & Copy-On-Write GEFS for OpenBSD**](https://www.phoronix.com/news/OpenBSD-GEFS-File-System) / [**'GEFS on OpenBSD: A very early preview'**](https://marc.info/?l=openbsd-tech&m=178948744271633) - Ori Bernstein's "good enough filesystem" now runs on OpenBSD, with the mailing-list post clear that it is a preview and not ready for production.
* [**shithub: the fragrant git host**](https://shithub.us/) - A Git host running git9 on 9front, where ori and other Plan 9 projects keep their repositories.
* [**Coreutils - rejected feature requests**](https://www.gnu.org/software/coreutils/rejected_requests.html) - The features coreutils has turned down over the years, with the reasoning behind each rejection.
* [**wwmm/easyeffects**](https://github.com/wwmm/easyeffects) - Limiter, compressor, convolver, equalizer and auto-volume plugins for PipeWire applications.
* [**omarchy-speaker-calibrator**](https://github.com/thefreshoffice/omarchy-speaker-calibrator) - Measures your speakers with a microphone and generates a validated, protective parametric calibration for the Omarchy bar.
* [**nixarchy**](https://github.com/olafkfreund/nixarchy/releases) - Omarchy 4.x vendored for NixOS as a derivation rather than reimplemented in Nix.

## Hardware & Homelab

* [**Converting a $20 4G wireless hotspot into a texting device**](https://bkovac.github.io/modem-thing/) - An OpenStick-compatible MF800 hotspot turned into something that can send SMS, assembled from parts already lying on the desk.
* [**EchoMuse**](https://github.com/wilbowes/EchoMuse) - An Alexa replacement and local controller for the second-generation Echo Dot.

## Security & Privacy

* [**LG statement on smart TV privacy**](https://www.lg.com/global/newsroom/news/statements/statement-understanding-privacy-on-lg-smart-tvs/) - LG's answer to the recent coverage: wake-word audio is processed locally and discarded, ACR is opt-in and off by default, and voice sessions are time-limited, with consent managed in TV settings.

## Gaming & Retro

* [**Sega Rally 2 ~ 25th Anniversary Edition**](https://archive.org/details/sega-rally-2-25th-anniversary) - A repack of the Dreamcast rally racer, in English, Spanish and Japanese.
* [**X-Men Origins: Wolverine - Uncaged Edition**](https://archive.org/details/x-men-origins-wolverine.-7z) - The uncut 2009 tie-in game, archived for download.
* [**The Gran Turismo Magazine: "Beyond the Apex"**](https://archive.org/details/GT6BeyondTheApexEn/) - The promotional magazine that shipped with Gran Turismo 6.
* [**I am stepping away from the PS5 Linux scene**](https://x.com/theflow0/status/2099987019954831744) - Andy Nguyen (theflow0) stops his PS5 Linux work, PS5 Pro support included.

## Releases & Misc

* [**Major updates for Apple's software platforms**](https://www.apple.com/newsroom/2026/09/major-updates-for-apples-software-platforms-are-now-available/) - Apple's annual OS releases are out, bringing Siri AI and new Apple Intelligence features.
* [**Canada welcomes EU proposal to become 'associate member'**](https://www.bbc.com/news/articles/cwly7vkke4jxo) - Mark Carney backs a Canada-EU alliance; the week's non-technical link.
