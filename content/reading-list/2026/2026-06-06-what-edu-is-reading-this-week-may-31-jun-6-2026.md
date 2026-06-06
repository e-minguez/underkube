---
title: "What Edu is reading this week (May 31 - Jun 6, 2026)"
date: 2026-06-06T10:00:00+02:00
draft: false
slug: 2026-06-06-what-edu-is-reading-this-week-may-31-jun-6-2026
aliases:
  - /posts/2026-06-06-what-edu-is-reading-this-week-may-31-jun-6-2026/
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
  - hardware
  - sdr
  - gaming
---

Running LLMs on a Game Boy Color and a £200 datacenter GPU, GPS jamming over Europe, npm supply chain compromise, aircraft tracking on your ceiling, and DOOM's kryptonite: the Neo Geo.

![What Edu is reading this week (May 31 - Jun 6, 2026)](/images/2026-06-06-what-edu-is-reading-this-week-may-31-jun-6.png)

## AI, Agents & Tools

* [**maddiedreese/gbc-transformer**](https://github.com/maddiedreese/gbc-transformer) / [**Reddit discussion**](https://www.reddit.com/r/LocalLLaMA/comments/1tbi2n3/i_got_a_real_transformer_language_model_running/): TinyStories-260K running locally on a stock Game Boy Color — no phone, PC, Wi-Fi, link cable, or cloud. The cartridge boots a ROM and the GBC runs the model itself.
* [**I Put a Datacenter GPU in My Gaming PC for £200**](https://blog.tymscar.com/posts/v100localllm/): A V100 that doesn't fit a normal motherboard, fan wired with jumper cables, running a model that benchmarks alongside Claude Sonnet 4.6 — for £200.
* [**A 10 year old Xeon is all you need**](https://point.free/blog/gemma-4-on-a-2016-xeon/): Gemma 4 on a 2016 Xeon, no GPU, 128 GB DDR3, 25 flags, and a 25B MoE model. No dedicated hardware required.
* [**Introducing Gemma 4 12B**](https://blog.google/innovation-and-ai/technology/developers-tools/introducing-gemma-4-12b/): Google's unified, encoder-free multimodal model designed to run on a laptop.
* [**PrismML — Bonsai Image 4B**](https://prismml.com/news/bonsai-image-4b): 1-bit and ternary quantized image generation model aimed at local, low-resource devices.
* [**jundot/omlx**](https://github.com/jundot/omlx): LLM inference server with continuous batching and SSD caching for Apple Silicon, managed from the macOS menu bar.
* [**mostlygeek/llama-swap**](https://github.com/mostlygeek/llama-swap): Reliable model swapping for any local OpenAI/Anthropic-compatible server — llama.cpp, vllm, and others.
* [**agent-substrate/substrate**](https://github.com/agent-substrate/substrate): Agent Substrate — a core system for building and running AI agents.
* [**stevesolun/ctx**](https://github.com/stevesolun/ctx): Skill, agent, MCP, and harness recommendations for Claude Code and custom LLMs — 102K-node LLM-wiki graph, 91K skills, 10K MCPs, 13 harnesses.
* [**rh-ai-quickstart/lemonade-stand-assistant**](https://github.com/rh-ai-quickstart/lemonade-stand-assistant): Red Hat's AI-powered customer service assistant with LLM guardrails and multiple detector models — the repo name itself is a live prompt injection example, which is a fitting meta-commentary for a guardrails project.
* [**Sites – Codex | OpenAI Developers**](https://developers.openai.com/codex/sites): Codex can now build and deploy hosted sites via a Sites plugin.
* [**Expanding Project Glasswing**](https://www.anthropic.com/news/expanding-project-glasswing): Anthropic extending its safety research program to ~150 new organizations across 15+ countries.

## Security

* [**Multiple redhat-cloud-services npm Packages compromised**](https://www.stepsecurity.io/blog/multiple-redhat-cloud-services-npm-packages-compromised): Packages in the `@redhat-cloud-services` npm scope carried malicious preinstall hooks — a multi-stage credential harvester targeting GitHub Actions secrets, AWS, GCP, Azure, Kubernetes, Vault, npm, and CircleCI tokens.
* [**1-Click GitHub Token Stealing via a VSCode Bug**](https://blog.ammaraskar.com/github-token-stealing/): A VSCode vulnerability that lets a malicious extension steal your GitHub token with a single click and no user prompt.
* [**Pwnd Blaster: Hacking your PC using your speaker without ever touching it**](https://blog.nns.ee/2026/06/03/katana-badusb/): Abusing an unauthenticated Bluetooth protocol to turn a PC speaker into a Rubber Ducky — BadUSB without the USB.

## Linux & Systems

* [**You Don't Love systemd Timers Enough**](https://blog.tjll.net/you-dont-love-systemd-timers-enough/): A solid case for replacing cron with systemd timers, with practical examples of where timers handle edge cases better.
* [**c0deJedi/nbd-vram**](https://github.com/c0dejedi/nbd-vram): Use your NVIDIA GPU's VRAM as swap space on Linux — built for laptops with soldered RAM that have an RTX card sitting largely idle.
* [**Knuckle: Flatcar Container Linux for the Home**](https://docs.projectbluefin.io/blog/introducing-knuckle/): Project Bluefin bringing Flatcar's immutable, container-focused OS to home servers and homelabs.
* [**kristapsdz/openrsync**](https://github.com/kristapsdz/openrsync): BSD-licensed rsync implementation — clean, readable, wire-compatible with the original.
* [**microsoft/coreutils**](https://github.com/microsoft/coreutils): Microsoft's packaging of GNU coreutils for Windows.
* [**pibylick/codecontainer**](https://github.com/pibylick/codecontainer): Isolated container environments for AI coding assistants (Codex, Claude Code, opencode) — supports Docker, Podman, and Apple Container.
* [**Adding a new package to openSUSE Leap and Package Hub**](https://youtube.com/watch?v=wM9NbrpxT4Q&is=zdzrfJOmK57rPbxU): Video walkthrough of the openSUSE packaging process from scratch.
* [**mainframed/Hackers-Plymouth**](https://github.com/mainframed/Hackers-Plymouth): Boot splash themes straight out of the 1995 Hackers movie.

## SDR, Hardware & Electronics

* [**Something is jamming GPS over Europe**](https://youtube.com/watch?v=tz23G_UXCGA&is=JHf3yLgryGQEoAvp): Investigation into GPS signal disruptions across Europe — sources, patterns, and what's actually causing them.
* [**Skylight — the sky, on your ceiling**](https://skylightceiling.com/) / [**cpaczek/skylight**](https://github.com/cpaczek/skylight): Project aircraft passing overhead onto your ceiling in real time using an RTL-SDR, with a live sky layer including sun, moon, stars, and the ISS.
* [**greystoke1337/localized-air-traffic-tracker**](https://github.com/greystoke1337/localized-air-traffic-tracker): Simple ADS-B project for tracking aircraft arriving at a specific airport.
* [**disketteomelette/cnafsdrsharp**](https://github.com/disketteomelette/cnafsdrsharp): Integration of the Spanish National Frequency Assignment Table (CNAF) into SDRSharp — useful for identifying what's on a given frequency in Spain.
* [**NeoCalculator: The €20 Open-Source Graphing Calculator**](https://neocalculator.tech/): ESP32-based open-source graphing calculator with a CAS engine — for €20.

## Development & Tools

* [**Stop Using Conventional Commits**](https://sumnerevans.com/posts/software-engineering/stop-using-conventional-commits/) / [**Scoped Commits**](https://scopedcommits.com/): Sumner Evans argues Conventional Commits focuses on the wrong things and fails its promises — alongside Scoped Commits, an alternative approach worth a look.
* [**Changing How We Develop Ladybird**](https://ladybird.org/posts/changing-how-we-develop-ladybird/): The Ladybird browser project changing its development model as it prepares to ship to real users.
* [**pandoc-templates.org**](https://pandoc-templates.org/): Collection of Pandoc templates for PDF, LaTeX, HTML, and Word documents.
* [**mouseless**](https://mouseless.click/): Practice tool for keyboard-only workflows — learn shortcuts and reduce mouse dependency.
* [**Chuwi Minibook X**](https://tylercipriani.com/blog/2026/05/28/chuwi-minibook-x/): Hands-on with the Chuwi Minibook X — a surprisingly capable ultracompact laptop at a fraction of the usual price.

## Gaming, Fun & Misc

* [**DOOM Runs On Everything...except Neo Geo**](https://www.youtube.com/watch?v=4f1-7c6WX10): The Neo Geo is a 2D sprite powerhouse but its architecture makes 3D rendering genuinely difficult — a deep-dive into why DOOM doesn't run on it.
* [**hampter-mods/pscstore-release**](https://github.com/hampter-mods/pscstore-release): A modern game management hub for the PlayStation Classic running Project Eris.
* [**WeRide, Uber and AVOMO Bring Robotaxis to Madrid**](https://finance.yahoo.com/sectors/technology/articles/weride-uber-avomo-bring-robotaxis-083000335.html?guccounter=1): Spain's first commercial robotaxi pilot launching in Madrid — WeRide and Uber's first joint European market entry.
* [**Meta scales back plan to track workers' clicks and keystrokes to train AI**](https://www.bbc.com/news/articles/c93x0k194yno): Following internal pushback, Meta adding a 30-minute pause option for employees being surveilled to train AI models.
* [**Rick C-137 vs Rick Prime: the facts**](https://www.reddit.com/r/rickandmorty/s/esNe9RxolK): A Reddit breakdown clearing up common confusion between the two Ricks in Rick and Morty.
