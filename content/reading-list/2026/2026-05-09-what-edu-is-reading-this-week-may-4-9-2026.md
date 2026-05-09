---
title: "What Edu is reading this week (May 4 - 9, 2026)"
date: 2026-05-09T10:00:00+02:00
draft: false
slug: 2026-05-09-what-edu-is-reading-this-week-may-4-9-2026
aliases:
  - /posts/2026-05-09-what-edu-is-reading-this-week-may-4-9-2026/
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

Another Linux LPE in the wild, OpenAI launches ads in ChatGPT, and a solid batch of self-hosted tooling covering monitoring, photo sharing, and pastebins.

## Security

* [**V4bel/dirtyfrag**](https://github.com/V4bel/dirtyfrag): Linux privilege escalation that chains the `xfrm-ESP` and `RxRPC` page-cache write vulnerabilities — deterministic (no race condition), affects ~9 years of kernel versions, and gains root on Ubuntu, RHEL, Fedora, and others. Same family as Dirty Pipe and Copy Fail.

## AI, Agents & Tools

* [**89luca89/clampdown**](https://github.com/89luca89/clampdown): Run AI coding agents in hardened container sandboxes — a useful containment layer for agentic workloads.
* [**dottorblaster/amake**](https://github.com/dottorblaster/amake): Task runner designed for AI CLI tools.
* [**Yet Another Openclaw vs Hermes experience sharing**](https://www.reddit.com/r/openclaw/s/euphAcvPVU): Community comparison of the two leading self-hosted personal AI agent frameworks — OpenClaw (Peter Steinberger, messaging-gateway-first, 250k stars) vs Hermes Agent (Nous Research, agent-first with a self-improving "reflective phase", 110k stars in ten weeks).
* [**OpenAI Ads**](https://ads.openai.com/): OpenAI launches an advertising platform inside ChatGPT — ads surfaced during product research and decision-making flows.
* [**Google Chrome silently installs a 4 GB AI model on your device**](https://www.thatprivacyguy.com/blog/chrome-silent-nano-install/): Chrome downloads Gemini Nano (4 GB) to user machines without consent, no opt-out short of enterprise tooling, re-downloads if deleted. Includes legal and environmental analysis at billion-device scale.

## Cloud, Kubernetes & Infrastructure

* [**We replaced our registry mirror scanner with a K8s admission webhook**](https://tinysystems.io/blog/admission-webhook-registry-mirror) / [**We built a self-healing registry mirror**](https://tinysystems.io/blog/registry-mirror-automation): Two-part series from Tiny Systems on building a self-healing zot registry mirror on GKE and intercepting image pulls at the API level via admission webhook — no more ImagePullBackOff, images rewritten before pods exist.

## Linux & Systems

* [**msmtp**](https://marlam.de/msmtp/) / [**msmtp - ArchWiki**](https://wiki.archlinux.org/title/Msmtp): Lightweight SMTP client for sending mail from scripts and CLI — simpler than a full MTA for most self-hosted setups.
* [**Glances**](https://nicolargo.github.io/glances/) / [**nicolargo/glances**](https://github.com/nicolargo/glances): Cross-platform system monitoring tool (top/htop alternative) with web UI and API — good fit for homelab dashboards.
* [**henrygd/beszel**](https://github.com/henrygd/beszel): Lightweight server monitoring with historical data, Docker stats, and alerts.
* [**openSUSE Manpages Server**](https://manpages.opensuse.org/): Online man page browser for openSUSE packages — handy reference.

## Self-hosted

* [**immich-app/immich — Partner Sharing Discussion**](https://github.com/immich-app/immich/discussions/7038) / [**ajb3932/immich-partner-sharing**](https://github.com/ajb3932/immich-partner-sharing) / [**alangrainger/immich-person-to-album**](https://github.com/alangrainger/immich-person-to-album): Community discussion on what partner sharing in Immich should actually cover, plus two tools that work around current gaps: one mirrors sharing state between partners, the other auto-adds people to albums so they can be shared.
* [**PrivateBin/PrivateBin**](https://github.com/PrivateBin/PrivateBin) / [**thomiceli/opengist**](https://github.com/thomiceli/opengist) / [**bhavnicksm/pbnj**](https://github.com/bhavnicksm/pbnj): Three self-hosted pastebin options — PrivateBin does zero-knowledge client-side AES encryption, opengist is Git-backed (open-source GitHub Gist alternative), pbnj is minimal.

## Networking & Hardware

* [**High quality router in Europe for €30?**](https://forum.openwrt.org/t/high-quality-router-in-europe-for-30/249640): OpenWrt forum thread on budget routers available in Europe — Cudy WR3000 series and Xiaomi AX3000T (EU RD23 version) come out as the top picks around €40, with good OpenWrt support and MediaTek SoCs.

## Development & Tools

* [**80 characters? In this economy?**](https://www.bitecode.dev/p/80-characters-in-this-economy): A look at why the 80-char line limit persists and whether it still makes sense today.

## Gaming, Fun & Misc

* [**The Gaming Emporium**](https://thegamingemporium.com/): Curated catalog of game decompilations, ports, and mods.
* [**Turning a $20 AliExpress clock into a real vintage Macintosh**](https://youtube.com/watch?v=zAbAf5-H5Yo) / [**wr/macintosh-mini**](https://github.com/wr/macintosh-mini) / [**macemu-jit**](https://rcarmo.github.io/projects/macemu-jit/): Pi Zero 2W + SheepShaver inside a Mac-shaped AliExpress alarm clock — runs classic Mac OS. Companion projects cover the emulator build and a pre-built Raspberry Pi .deb.
