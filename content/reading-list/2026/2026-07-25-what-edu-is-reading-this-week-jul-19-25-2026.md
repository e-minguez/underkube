---
title: "What Edu is reading this week (Jul 19 - 25, 2026)"
date: 2026-07-25T10:00:00+02:00
draft: false
slug: 2026-07-25-what-edu-is-reading-this-week-jul-19-25-2026
aliases:
  - /posts/2026-07-25-what-edu-is-reading-this-week-jul-19-25-2026/
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

A week of open-weight model routing and local AI tooling, OCI-backed package managers and registries, a Linux kernel CVE deluge, self-hosting mail and media, plus a good run of retro-computing and hardware rabbit holes.

## AI, Models & Agents

* [**Kimi K3 is competitive with Fable; Kimi K3 + Fable is SoTA**](https://fireworks.ai/blog/kimik3-fable): Fireworks benchmarks routing between the open-source Kimi K3 and the closed Fable across 1,000+ agentic tasks, arguing a router that plays to each model's strengths beats either alone.
* [**Echo by Tracer**](https://echo.tracerml.ai/) / [**Show HN**](https://news.ycombinator.com/item?id=49026810): Echo pitches Fable-level results at a third of the cost using open-weight models, with the Show HN thread for discussion.
* [**Introducing Gemini 3.6 Flash, 3.5 Flash-Lite, and 3.5 Flash Cyber**](https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-3-6-flash-3-5-flash-lite-3-5-flash-cyber/): Google introduces three new Gemini models, including a Flash Cyber variant.
* [**Claude Cookbook**](https://platform.claude.com/cookbook/): Practical guides and code examples for building with Claude — prompting techniques, tool use and multimodal capabilities.
* [**ComposioHQ/composio**](https://github.com/composiohq/composio/): 1000+ toolkits, tool search, context management, authentication and a sandboxed workbench for building AI agents that turn intent into action.
* [**Nativ — Run AI locally on your Mac**](https://blaizzy.github.io/nativ/): Run frontier models locally on your Mac — no accounts, subscriptions or cloud.
* [**Libvirt Powered Claude Sandbox**](https://gist.github.com/smith153/04b4068b5a2d7b234f1c3d5992dafe25): A gist for running Claude inside a libvirt-backed VM sandbox.
* [**I Fine-Tuned a 7B Model to Be a Cloud Security Expert On My Local Machine, For $0**](https://blog.valqore.io/i-fine-tuned-a-7b-model-to-be-a-cloud-security-expert-on-my-local-machine-for-0-ec77fe491703): Fine-tuning a 7B model into a cloud-security assistant locally in 43 minutes on a consumer GPU, with 3,298 training pairs and no API cost.
* [**podcast-shorts-factory**](https://github.com/krakonjac300-pixel/podcast-shorts-factory) / [**Write-up**](https://www.reddit.com/r/AI_Agents/comments/1v3d7vy/i_spent_a_month_building_10_ai_agents_that_run_a/): Ten cooperating AI agents that turn long podcasts into short-form videos automatically, open source and running on free AI providers.
* [**Stop Using OpenCode**](https://wren.wtf/shower-thoughts/stop-using-opencode/): A shower-thoughts blog post making the case against OpenCode.
* [**"You can use the Opus to jailbreak the Opus"**](https://x.com/elder_plinius/status/2045682830383231474): An X thread claiming an agent wrote a universal jailbreak from scratch and used computer use to validate it against Opus.

## Cloud, Kubernetes & Infrastructure

* [**ttl.sh — Anonymous & Ephemeral OCI Registry**](https://ttl.sh/): A free, anonymous, ephemeral OCI registry — push images with no sign-up and they expire automatically.
* [**Introducing pkgoci**](https://ericcurtin.github.io/pkgoci/blog/2026-07-17-introducing-pkgoci.html): A fast, native package manager where every package is an OCI artifact, backed by OCI registries (Docker Hub by default), for macOS, Linux and Windows.
* [**Sylve — Management Plane for FreeBSD**](https://sylve.io/): A modern web interface for FreeBSD — unified management of Bhyve VMs, jails, ZFS storage, networking and system monitoring.

## Linux & Systems

* [**FreeBSD ports frozen after someone commits the entire 150MB Linux Copilot binary**](https://www.osnews.com/story/145593/freebsd-ports-frozen-after-someone-commits-the-entire-150mb-linux-copilot-binary/): The FreeBSD ports tree froze after someone committed the whole 150MB Linux Copilot binary.
* [**A moment of silence, please, for the final release of Debian on x86-32**](https://www.theregister.com/os-platforms/2026/07/15/a-moment-of-silence-please-for-the-final-release-of-debian-on-x86-32/5271198): The Register marks the final Debian release supporting 32-bit x86, alongside the 13.6 and 12.15 point releases.
* [**432 Linux kernel CVEs published in the last 24 hours**](https://lobste.rs/s/t2jxyu/432_linux_kernel_cves_published_last_24) / [**Archive**](https://lore.kernel.org/linux-cve-announce/): 432 Linux kernel CVEs published in a single 24-hour window, with the linux-cve-announce archive to browse them.
* [**roadkell/ascii-logos**](https://github.com/roadkell/ascii-logos) / [**Boot screen**](https://github.com/Yilmaz41/Thinkpad-boot-screen): ThinkPad ASCII logos for your terminal, plus a matching Plymouth boot screen styled after Omarchy.

## Security

* [**Nextcloud leaks 367K records, exposing staff and clients**](https://cybernews.com/security/nextcloud-cloud-provider-data-leak/): A misconfigured database exposed 367K records — employee data, client contracts and infrastructure scripts — raising phishing risk.
* [**PortProtonQt: Custom Polkit Rule Allows Escalation (CVE-2026-59678)**](https://security.opensuse.org/2026/07/22/port-proton-qt-polkit-rules.html): A custom Polkit rule shipped by PortProtonQt lets any local user modify NetworkManager connections or UDisks2 mounts.
* [**OpenAI and Hugging Face partner to address security incident during model evaluation**](https://openai.com/index/hugging-face-model-evaluation-security-incident/): OpenAI and Hugging Face share early findings from a security incident during AI model evaluation, and lessons for defenders.

## Self-Hosting & Homelab

* [**You should selfhost your mail**](https://blog.haschek.at/2026/you-should-selfhost-your-mail.html): Christian Haschek on why — and how — to self-host your email.
* [**Nomad: The World's Smallest Media Server**](https://www.reddit.com/r/homelab/s/gYSAZ00iRm): An open-source media server with movies, books, music, maps, games and offline Wikipedia.
* [**The death and rebirth of my home server**](https://sgt.hootr.club/blog/home-server-rebirth/): A blogger rebuilds their home server from the ground up.
* [**Free Ink · An open ecosystem for e-readers**](https://freeink.org/): Open-source software, firmware and hardware for e-paper readers — every layer shipped in the open.

## Development, Web & Tools

* [**I Regret Migrating to Codeberg**](https://xn--gckvb8fzb.com/i-regret-migrating-to-codeberg/): A short argument on why a free-software host deciding which projects are welcome worries the author more than the bans themselves.
* [**Jelly UI — Soft Web Components**](https://jelly-ui.com/): A dependency-free Web Components library for tactile interfaces — soft-body physics, real form controls, dark mode, RTL and WCAG AA accessibility.
* [**GitHub suddenly rejected my SSH key (the fix was a .pub file?!)**](https://thorsell.io/2026/07/21/github-ssh-keys.html): git pull stopped working with permission denied out of nowhere — and the fix turned out to involve the .pub file.
* [**is-a.dev Documentation**](https://docs.is-a.dev/): Docs for is-a.dev — guides, the JSON file structure and how to claim a free developer subdomain.

## Hardware, Retro & Fun

* [**DOSCON: A Handheld MS-DOS Machine Running on Two AAA Batteries**](https://blog.ikejima.org/make/8088/2026/07/21/doscon-en.html): A handheld MS-DOS machine built around an 8088 that runs on two AAA batteries.
* [**The Beam Engine — An Interactive Guide**](https://glinscott.github.io/beam-engine/): Interactive 3D figures explaining how a beam engine works — steam, pressure, Watt's condenser, valves, linkages and the governor.
* [**PCjs Machines**](https://www.pcjs.org/): Browser-based emulators for DOS, Windows, OS/2 and other vintage machines, plus an archive of historical software and documentation.
* [**coelhomarcus/usagi-pkgj**](https://github.com/coelhomarcus/usagi-pkgj): PKG download and installation directly on the PS Vita.
* [**I wrote an API client for my water-cooled bed**](https://tinkering.xyz/bedctl/): Yes, really — a small API client (bedctl) for controlling a water-cooled bed.
* [**It's getting harder to focus every day**](https://glyphack.com/attention/): A personal essay on how hard it has become to hold attention, and forcing focus to get anything done.
