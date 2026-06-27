---
title: "What Edu is reading this week (Jun 21 - 27, 2026)"
date: 2026-06-27T07:00:00+02:00
draft: false
slug: 2026-06-27-what-edu-is-reading-this-week-jun-21-27-2026
aliases:
  - /posts/2026-06-27-what-edu-is-reading-this-week-jun-21-27-2026/
categories:
  - Reading
tags:
  - newsletter
  - links
  - tech
  - devops
  - linux
  - ai
  - security
  - kubernetes
  - sdr
---

A week mixing local LLM tooling, terminal-driven virtualization, OCI registries and PXE boot servers, a few BSD and mobile Linux releases, and some hardware tinkering.

## AI, Models & Coding

* [**microgpt**](https://gist.github.com/karpathy/8627fe009c40f57531cb18360106ce95): Karpathy's minimal GPT implementation in a single gist, for understanding the architecture from the ground up.
* [**vLLM + LMCache: A Starter Guide, No GPU Required**](https://blog.lmcache.ai/en/2026/06/23/vllm-lmcache-a-starter-guide-no-gpu-required/): A contributor-focused walkthrough of vLLM + LMCache on a single MacBook, covering the frontend, L1 eviction, L2 storage, and observability — no GPU needed.
* [**GLM-5.2 - How to Run Locally**](https://unsloth.ai/docs/models/glm-5.2): Unsloth's guide to running Z.ai's new GLM-5.2 model on local hardware.
* [**Is AI ruining our skills?**](https://www.nature.com/articles/d41586-026-01947-1): Nature reports on early studies showing that reliance on AI tools degrades the abilities of physicians and software engineers.
* [**Codex SQLite feedback logs can write ~640 TB/year**](https://github.com/openai/codex/issues/28224): An OpenAI Codex issue where the local SQLite feedback log writes a continuous flood of data, rapidly consuming SSD endurance.
* [**Understand Anything**](https://understand-anything.com/): Turns any codebase into an interactive knowledge graph you can explore, search, and learn from.

## Cloud, Containers & Infrastructure

* [**project-zot/zot**](https://github.com/project-zot/zot): A scale-out, production-ready, vendor-neutral OCI-native container image and artifact registry built purely on the OCI Distribution Specification.
* [**Deploying OpenClaw on Kubernetes with Helm**](https://serhanekici.com/openclaw-helm.html): OpenClaw's shell access and untrusted input create real attack surface — this guide deploys it on Kubernetes with Helm and ArgoCD so container isolation and network policies contain the blast radius.
* [**Running microVMs in Proxmox VE, The Easy Way**](https://taoofmac.com/space/blog/2026/06/18/1845) / [**VirtUI Manager**](https://aginies.github.io/virtui-manager/): Running lightweight microVMs across a mixed Proxmox cluster, plus VirtUI Manager, a next-generation terminal-based UI for managing QEMU/KVM virtual machines.
* [**Bootimus — Modern PXE/HTTP boot server**](https://bootimus.com/): A self-contained PXE and HTTP boot server in a single binary with zero config and 50+ distros out of the box.

## Linux & Systems

* [**Announcing NetBSD 11.0 RC5**](https://www.netbsd.org/releases/formal-11/NetBSD-11.0.html): The fifth release candidate for NetBSD 11.0, out June 16, 2026.
* [**postmarketOS v26.06: Alpen Avocado**](https://postmarketos.org/blog/2026/06/21/v26.06-release/): The latest postmarketOS release, aiming for a 10-year life-cycle for smartphones.
* [**Samsung SSD Firmware**](https://wiki.gentoo.org/wiki/Samsung_SSD_Firmware): The Gentoo wiki page on updating Samsung SSD firmware from Linux.

## Development, Web & Security

* [**Developers don't understand CORS**](https://fosterelli.co/developers-dont-understand-cors): The recent Zoom vulnerability is one of many examples showing how poorly CORS is understood, with a clear walkthrough of how it actually works.
* [**ivorpad/mercadona-cli**](https://github.com/ivorpad/mercadona-cli): An unofficial single-binary Go CLI to search the catalog, read prices, build a cart, and check out from Spain's Mercadona supermarket, with structured JSON output for scripting.

## SDR, Hardware & Misc

* [**The Xteink X4 E-Ink Reader**](https://blog.omgmog.net/post/xteink-x4-e-ink-reader/): A hands-on with the Xteink X4, a £40 e-ink reader small enough to stick to the back of a phone.
* [**ATS MiniRadio with RTTY, CW, WeFax, SSTV**](https://peterneufeld.wordpress.com/2026/06/08/wefax-sstv-for-ats-miniradio-v1-to-v4b/): A modification for SI4732 ATS MiniRadios (V1 to V4B) to decode SSTV and WeFax picture transmissions.
* [**Unlag Neo: Macbook Neo Cursor lag "fix"**](https://gist.github.com/retroplasma/ec21767d0a8380c7ea9c2fbee1c7d6bf): A gist with a workaround for the cursor lag on the MacBook Neo.
</content>
</invoke>
