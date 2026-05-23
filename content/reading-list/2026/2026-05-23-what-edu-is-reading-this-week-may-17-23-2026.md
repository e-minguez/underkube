---
title: "What Edu is reading this week (May 17 - 23, 2026)"
date: 2026-05-23T10:00:00+02:00
draft: false
slug: 2026-05-23-what-edu-is-reading-this-week-may-17-23-2026
aliases:
  - /posts/2026-05-23-what-edu-is-reading-this-week-may-17-23-2026/
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
---

Heavy FreeBSD week — a new kernel LPE (CVE-2026-45250), a decade-long Ubuntu migration story, and OpenBSD 7.9 out. Also: Flipper One opens up community development, a self-healing WireGuard mesh, and tools for stripping AI watermarks.

![What Edu is reading this week (May 17 - 23, 2026)](/images/2026-05-23-what-edu-is-reading-this-week-may-17-23.png)

## AI, Agents & Tools

* [**microsoft/AI-Engineering-Coach**](https://github.com/microsoft/AI-Engineering-Coach): Microsoft's toolkit for better agentic engineering — patterns, prompts, and workflows aimed at improving what AI agents actually do, not just how they're wired up.
* [**automateyournetwork/netclaw**](https://github.com/automateyournetwork/netclaw/tree/main): AI agent that interrogates your network — polls devices, collects data, and answers questions about your infrastructure through a conversational interface.
* [**MinishLab/semble**](https://github.com/MinishLab/semble): Fast semantic code search for AI agents — claims ~98% fewer tokens than grep+read while maintaining accuracy. Useful for agentic coding pipelines navigating large repos.
* [**wiltodelta/remove-ai-watermarks**](https://github.com/wiltodelta/remove-ai-watermarks): CLI and library for stripping visible (Gemini) and invisible (SynthID, C2PA, EXIF) AI watermarks from images.
* [**A new generation of ads for the AI era of Search**](https://blog.google/products/ads-commerce/google-marketing-live-search-ads/): Google announces new ad formats built with Gemini inside AI-powered Search — ads are now embedded in the AI overview, not just the sidebar.
* [**We let AIs run radio stations**](https://news.ycombinator.com/item?id=48183301): HN thread on fully AI-run radio stations — automated programming, DJ banter, and song selection, with the usual community debate around what this means for human radio.
* [**DecayDock – AI Smart Fridge Companion**](https://www.instructables.com/DecayDock-AI-Smart-Fridge-Companion/) / [**DecayDock: The Tiny AI Device That Combats Food Waste**](https://www.hackster.io/news/decaydock-the-tiny-ai-device-that-combats-food-waste-3a34ddad9cbf): ESP32-CAM + TFT display that tracks food freshness in your fridge using local AI. The Instructables post has the build; Hackster covers the concept.

## Security

* [**FatGid - FreeBSD 14.x kernel LPE**](https://fatgid.io/) / [**venglin/setcred: CVE-2026-45250**](https://github.com/venglin/setcred): A four-byte type confusion in a credential-handling syscall yields a root shell on FreeBSD 14.x. The landing page is concise; the PoC repo has the full exploit code.
* [**0xdeadbeefnetwork/ssh-keysign-pwn**](https://github.com/0xdeadbeefnetwork/ssh-keysign-pwn): Exploits the ptrace_may_access mm-NULL bypass + pidfd_getfd to steal SSH host private keys and `/etc/shadow` on pre-31e62c2ebbfd kernels.
* [**pocs/fragnesia**](https://github.com/v12-security/pocs/tree/main/fragnesia-5db89c99566fc): PoC from v12-security's collection — details are sparse in the repo description, worth tracking if you follow their work.
* [**Alcoholless**](https://medium.com/nttlabs/alcoholless-a-lightweight-security-sandbox-for-macos-programs-homebrew-ai-agents-etc-ccf0d1927301) / [**AkihiroSuda/alcless**](https://github.com/AkihiroSuda/alcless): Lightweight security sandbox for macOS — restricts network and filesystem access for Homebrew packages, AI agents, and other untrusted programs without needing a VM.

## Cloud, Kubernetes & Infrastructure

* [**cgroups: From Chaos to Control**](https://rawkode.academy/read/cgroups-from-chaos-to-control): Deep dive into Linux cgroups v1 vs v2 — the history, the architectural differences, and what it means for Kubernetes workloads. Solid foundation piece.
* [**encodeous/nylon**](https://github.com/encodeous/nylon): Self-healing WireGuard mesh — reroutes around failures in seconds with no coordination server and no cloud dependency. Fully FOSS.
* [**alebeck/boring**](https://github.com/alebeck/boring): Minimal SSH tunnel manager with config-file-defined named tunnels and auto-reconnect. Does one thing well.
* [**ttlequals0/MinusPod**](https://github.com/ttlequals0/MinusPod): Self-hosted server that strips ads from podcast feeds before playback — no client-side plugins required, works with any podcast app.

## Linux & Systems

* [**OpenBSD 7.9**](https://www.openbsd.org/79.html): OpenBSD 7.9 released — new hardware support, kernel improvements, and the usual security hardening pass.
* [**The FreeBSD Project**](https://www.freebsd.org/): FreeBSD.org got a redesign — worth a look if you haven't visited in a while.
* [**This blog ran on Ubuntu 16.04 for 10 years. I migrated it to FreeBSD**](https://crocidb.com/post/this-blog-ran-on-ubuntu-16-04-for-10-years-i-migrated-it-to-freebsd/): Migration notes from a decade on Ubuntu 16.04 to FreeBSD on Hetzner — covers jails, Bastille, Caddy reverse proxy, and cross-continent load testing results.
* [**Announcing Web Serial Support in Firefox**](https://hacks.mozilla.org/2026/05/web-serial-support-in-firefox/): Firefox 151 ships the Web Serial API for desktop — browsers can now talk directly to microcontrollers, 3D printers, power meters, and other serial-connected hardware.
* [**clefspear/starcommand**](https://github.com/clefspear/starcommand): Generative terminal greeting — spawns a unique, deterministic rocket artwork on every new shell session across bash, zsh, fish, and PowerShell.

## Development & Tools

* [**Slumber**](https://slumber.lucaspickering.me/): TUI HTTP client — define, execute, and share configurable HTTP requests from the terminal. Requests live in config files, so they're version-controllable.
* [**zakirullin/files.md**](https://github.com/zakirullin/files.md): Personal knowledge system built on plain `.md` files — no app lock-in, no database, just directories and text.
* [**indaco/malt**](https://github.com/indaco/malt): Fast Homebrew alternative for macOS — warm installs in milliseconds, `post_install` scripts that actually run. Drop-in replacement.

## Hardware, Electronics & Fun

* [**Flipper One — we need your help**](https://blog.flipper.net/flipper-one-we-need-your-help/) / [**Tech specs - Flipper One**](https://docs.flipper.net/one/general/tech-specs): Flipper opens up Flipper One development to the community — a full Linux cyberdeck in Flipper form factor. The tech specs page has the hardware breakdown.
* [**BlueSCSI Images**](https://bluescsi.com/docs/BlueSCSI-Images#Macintosh): Curated disk images for BlueSCSI v2, with a dedicated Macintosh section — useful if you're running BlueSCSI in a vintage Mac and want pre-built system images.
* [**Was my $48K GPU server worth it?**](https://rosmine.ai/2026/05/13/was-my-48k-gpu-worth-it/): An independent researcher's honest accounting of building a 6×6000 Ada GPU server after leaving FAANG — build notes, problems encountered, and whether the investment paid off for AI research.
* [**andrzej3393/oldputer**](https://github.com/andrzej3393/oldputer): ESP32 + WeAct 4.2" e-paper display built to look like a vintage computer — retro aesthetic, low power, interesting case design.
* [**kageroumado/phosphene**](https://github.com/kageroumado/phosphene): Video wallpaper engine for macOS Tahoe — plays video files as your desktop background, a feature macOS doesn't support natively.
* [**Capsolver**](https://www.capsolver.com/): AI-powered CAPTCHA solving service — supports reCAPTCHA, Cloudflare, AWS WAF, OCR, and more. Worth knowing about for automation and testing workflows.
