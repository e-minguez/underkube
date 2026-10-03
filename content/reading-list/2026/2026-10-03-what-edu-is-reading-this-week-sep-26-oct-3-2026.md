---
title: "What Edu is reading this week (Sep 26 - Oct 3, 2026)"
date: 2026-10-03T09:00:00+02:00
draft: false
slug: 2026-10-03-what-edu-is-reading-this-week-sep-26-oct-3-2026
aliases:
  - /posts/2026-10-03-what-edu-is-reading-this-week-sep-26-oct-3-2026/
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
  - homelab
  - gaming
  - sdr
---

Two frontier model releases landed this week next to a batch of agent runtimes and small decision models, and the open-weights GLM-5.3 release came with a security assessment worth reading. On the systems side there is homelab storage, Linux on Apple Silicon, ZFS tuning, and a good amount of PS5 and 3D printing tinkering.

## AI, Agents & Models

* [**Pi 1.0**](https://earendil.com/posts/pi-1-0/) / [**Pi Durable**](https://earendil.com/posts/pi-durable/) - The 1.0 release of a minimal, hardened agent harness, plus an experimental substrate for long-running, durable agents that can run anywhere.
* [**"You Said No MCP!"**](https://earendil.com/posts/you-said-no-mcp/) - Why Pi reversed its position and now supports MCP, what changed in the protocol and in Pi, and what Codemode is.
* [**Gemini 4 Argon: our next era of frontier intelligence**](https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-4-argon/) - Google's new frontier model for real-world coding, enterprise knowledge work and cyber defense, rolling out soon.
* [**Introducing Claude Sonnet 5.5**](https://www.anthropic.com/claude-sonnet-5-5) - Anthropic's mid-tier refresh, which it says runs more than 30% faster and costs up to 30% less than Sonnet 5 on most work.
* [**zai-org/GLM-5.3**](https://huggingface.co/zai-org/GLM-5.3) / [**GLM-5.3 and the spread of advanced cyber capabilities**](https://www.anthropic.com/research/glm-5-3-and-the-spread-of-advanced-cyber-capabilities) - The open-weights release, and Anthropic's assessment that it can autonomously build end-to-end cyber exploits and shipped without meaningful safeguards against misuse.
* [**Ollama now supports Jev-style decision models**](https://ollama.com/blog/ollama-now-supports-jev-style-decision-models) - Decision models based on TypeSafe's Jev API now run locally at no cost, answering yes or no questions, choices and scores with a probability for every option.
* [**Introducing dots**](https://openai.com/index/introducing-dots/) - OpenAI's proactive assistants, built to keep working across complex projects and everyday tasks.
* [**firelex/jeff**](https://github.com/firelex/jeff) - Fine-tunes of Qwen3.5 and Gemma 4 for zero-shot classification: a 0.8B "System 1" model that picks between your options in milliseconds.
* [**Anthropic: Net loss of 42 billion US dollars in 2025 alone**](https://www.heise.de/en/news/Anthropic-Net-loss-of-42-billion-US-dollars-in-2025-alone-11468935.html) - What the company's stock prospectus discloses about its spending and losses.
* [**The AI Race Just Got Awkward**](https://insufferable.dev/posts/the-ai-race-just-got-awkward/) - A short piece on how quiet the field went after the latest round of frontier releases.

## Cloud, Homelab & Storage

* [**Meet the X4 | 45Homelab Unraid Signature Series**](https://unraid.net/shop-prebuilts/x4) - A compact four-bay Unraid server for media, files, apps and everyday projects.
* [**Oberiz**](https://github.com/anjelohe/Oberiz) - Self-hosted media automation for movies and series.
* [**Biggest ZFS Misconfigurations and How to Fix Them: Part 1**](https://klarasystems.com/articles/zfs-misconfigurations-how-to-fix-part-1/) - Walks through ashift, recordsize, vdev layout, dedup and pool capacity, and how each one typically goes wrong.
* [**ZFS Dataset Tuning**](https://lzon.ca/posts/tips/zfs-dataset-tuning/) - Practical notes on tuning ZFS datasets.

## Linux & Systems

* [**Debian alert DSA-6528-1 (kernel)**](https://lwn.net/Articles/1097401/) - The kernel security update advisory for Debian.
* [**Google breaks promise to provide 10 years of updates to Chromebooks**](https://www.osnews.com/story/146052/google-breaks-promise-to-provide-10-years-of-updates-to-chromebooks/) - OSnews on how the long update guarantee is being cut back.
* [**Gravity Linux**](https://gravitylinux.org/) / [**Asahi fork embraces LLMs and lands Linux on the M4 Mac mini**](https://www.theregister.com/os-platforms/2026/09/25/asahi-fork-embraces-llms-and-lands-linux-on-the-m4-mac-mini/5298931) - A Fedora remix for modern Apple Silicon Macs, and how coding agents helped two developers bring up an accelerated desktop and graphics driver on the M4 Mac mini in weeks.
* [**t1-touchbar**](https://github.com/AJ-dev-i60/t1-touchbar) - A DKMS kernel driver that makes the 2016 to 2017 MacBook Pro Touch Bar work on Linux, freeze-safe by default and building on kernel 7.x.
* [**CoW, a stacking window manager for Wayland**](https://cow-wm.codeberg.page/cow/) - A configurable stacking window manager built on River and inspired by FVWM and MWM.
* [**Re: [NEW] sysutils/uutils**](https://www.mail-archive.com/ports%40openbsd.org/msg143892.html) - The OpenBSD ports thread proposing uutils, the Rust coreutils rewrite, as a port.

## Mobile & Phones

* [**Project rebrand: Nura**](https://nura.eco/blog/2026/09/27/nura-rename/) / [**The road to daily-drivable mainline phones**](https://nura.eco/blog/2026/09/29/road-to-main-category/) - The project's new name and its plan for a ten year life cycle for smartphones running mainline Linux.

## Development & Web

* [**Destroy Any Website**](https://destroy.spritefusion.com/) - Feed it a URL and its text, images and boxes become a destructible pixel-art level you can play solo or with friends.
* [**IANA's email about why example.com changed**](https://www.oliverdunk.com/2026/09/30/iana-reply) - Oliver Dunk asked IANA about the new content on example.com, and their VP replied.
* [**Compositor**](https://github.com/robbietilton/Compositor) - An open source Photoshop alternative for macOS.

## SDR, Hardware & 3D Printing

* [**f5oeo on X (eSpDR)**](https://x.com/F5OEOEvariste/status/2105321268643832023) - Testing a 15 euro ESP32 for 80 MHz of spectrum at 2.4 GHz, decoding DATV and Wi-Fi, with I/Q capture and transmit as the next step.
* [**JBR-001: A Desktop Companion Robot Powered by Arduino UNO Q**](https://projecthub.arduino.cc/syntheticaidata/jbr-001-a-desktop-companion-robot-powered-by-arduino-uno-q-b11c96) / [**Show HN discussion**](https://news.ycombinator.com/item?id=49890707) - An open source, 3D printable desktop robot for exploring robotics, computer vision and edge AI.
* [**Klipper config for the Ender-3 V3 SE**](https://github.com/0xD34D/ender3-v3-se-klipper-config) / [**Ultimate Guide for Klipper Installation on Ender 3 V3 SE**](https://athemis.me/projects/klipper_guide/) - A working config plus a step-by-step install guide for running Klipper on the Ender 3 V3 SE.

## Gaming

* [**PS5: cómo ejecutar el jailbreak Relapse en la consola**](https://www.elotrolado.net/noticias/scene/playstation-5-exploit-relapse-disponible) - How to run the Relapse exploit on PS5 and PS5 Pro up to firmware 13.60, with payload and homebrew support.
* [**Hijacking the PS5's RTMP Stream**](https://yashgarg.dev/posts/hijacking-ps5-rtmp-stream/) - The long way around to screen sharing from the console.
* [**Xbox One y Xbox Series: digitalizar los juegos en formato físico**](https://www.elotrolado.net/noticias/juegos/xbox-licencias-disco-a-digital-disponible) - The disc-to-digital licence feature is now available to all Xbox users.
* [**ps5-portal-high-bitrate**](https://github.com/atameric/ps5-portal-high-bitrate) - Experimental 65, 100 and 200 Mbps bitrate targets for PS5 Remote Play on the PlayStation Portal via macOS, no jailbreak needed.
* [**PicoDate (PICO-8 Emulator for Playdate)**](https://bitcalibergames.itch.io/picodateplaydate) - An experimental MVP that plays PICO-8 carts on the Playdate, with Wi-Fi downloads and monochrome graphics.
* [**Lurikara (@Lurikara131) on X**](https://x.com/Lurikara131/status/2104929940168966353) - A thread noting that Gran Turismo 7's visuals appear to have dropped in quality after a recent update.

## Finanzas personales

* [**Cuenta Financia Europa: qué es, cómo funciona y cuándo se podrá contratar**](https://www.finect.com/usuario/eduardogarcia/articulos/cuenta-financia-europa-que-es-como-funciona-y-cuando-se-podra-contratar) / [**Simulador de la Cuenta Financia Europa**](https://simuladorfinanciaeuropa.com/) - What the new savings and investment account is, how it is taxed and when it can be opened, plus a calculator that compares the IRPF saving against a normal account.

## Science & Fun

* [**Scientists capture high-speed, full-colour footage of fusion plasma**](https://www.reddit.com/r/nextfuckinglevel/comments/1wtgjjl/scientists_have_captured_the_first_ever_highspeed/) - Slow-motion colour footage of plasma swirling inside a working reactor.
* [**Dauren Altynbek en Instagram**](https://www.instagram.com/reel/Dd2u0qqM0Wp/) - "Claude feat. his ex", an AI-generated clip made with Higgsfield Genjutsu.
