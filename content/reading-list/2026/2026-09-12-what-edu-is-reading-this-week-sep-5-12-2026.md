---
title: "What Edu is reading this week (Sep 5 - 12, 2026)"
date: 2026-09-12T09:00:00+02:00
draft: false
slug: 2026-09-12-what-edu-is-reading-this-week-sep-5-12-2026
aliases:
  - /posts/2026-09-12-what-edu-is-reading-this-week-sep-5-12-2026/
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
  - kubernetes
  - hardware
  - sdr
  - homelab
  - networking
  - gaming
---

A quieter week than the last one: open-weight audio tooling, Kubernetes checklists and Helm scanning, BSD install write-ups, a batch of homelab and SDR projects, and the Omarchy funding and vulnerability-disclosure threads.

## AI, Agents & Tools

* [**hexgrad/Kokoro-82M**](https://huggingface.co/hexgrad/Kokoro-82M) - An 82M-parameter open-weight text-to-speech model, small enough to run locally and to fine-tune.
* [**santinic/audiblez**](https://github.com/santinic/audiblez) - Generates audiobooks from EPUB e-books chapter by chapter, using Kokoro for the voices.
* [**DeepSeek-V4.1-Flash**](https://x.com/deepseek_ai/status/2097930608790167907) - The smallest model in DeepSeek's new architecture family, with native visual understanding and faster inference.
* [**Scenarios for our Economic Future**](https://www.anthropic.com/institute/econ-scenarios) - Anthropic's economics team models how AI could shape the economy of 2030.
* [**Claude Code for Everything**](https://hannahstulberg.substack.com/p/claude-code-for-everything-finally) - A beginner-oriented setup walkthrough: editor, working directory, terminal basics and skills, no coding required.
* [**ayghri/i-have-adhd**](https://github.com/ayghri/i-have-adhd) - A coding-agent skill that pushes the answer to the top instead of burying it under reasoning.

## Cloud, Kubernetes & Infrastructure

* [**kubernetes-production-best-practices**](https://github.com/learnk8s/kubernetes-production-best-practices) - learnk8s' checklist of the things to go over before releasing a workload to production.
* [**Scanning Helm Charts at Scale with helmsniff**](https://vahid-r.com/posts/helmsniff-tutorial/) - A walkthrough of scanning chart repositories for security issues.
* [**basarsubasi/kampfire**](https://github.com/basarsubasi/kampfire) - A Docker-style CLI for managing Kubernetes agent sandboxes with familiar commands.
* [**kj187/jarvis**](https://github.com/kj187/jarvis) - Self-hosted, realtime web frontend for Prometheus Alertmanager.

## Linux & BSD

* [**Stop making swap partitions**](https://gist.github.com/joshenders/c4960cec9c63a7b7d68ffa9543356c43) / [**Btrfs swapfile documentation**](https://btrfs.readthedocs.io/en/latest/Swapfile.html) - The case for a swapfile over a dedicated partition, with the Btrfs caveats from the docs.
* [**nixietab/vlcro**](https://github.com/nixietab/vlcro) - Makes zypper faster by running its slow operations in parallel.
* [**One Page, Every Package**](https://news.opensuse.org/2026/09/09/one-page-every-package/) / [**Tumbleweed vs Leap - osdiff**](https://opensuse.github.io/osdiff/) - openSUSE's answer to "which version of X do I actually get?", plus the tool that diffs source package versions between Tumbleweed and Leap.
* [**Omarchy's funding and the foundation**](https://www.reddit.com/r/omarchy/comments/1waskdz/omarchys_funding_dhhs_approach_the_foundation_and/) / [**Omarchy to drop Arch for NixOS?**](https://www.reddit.com/r/omarchy/s/BW3OH1SgCb) / [**Chainfire on the uncredited patches**](https://x.com/ChainfireXDA/status/2097244132783583561) - The community discussion on DHH's funding and governance approach, and the follow-up about privately reported vulnerabilities being patched without credit.
* [**NetBSD 11 from scratch**](https://meanmicio.org/2026/09/06/netbsd-11-from-scratch/) - Installing NetBSD by hand instead of with sysinst, full-disk encryption included.
* [**AMD Based FreeBSD Desktop Reloaded**](https://vermaden.wordpress.com/2026/09/06/amd-based-freebsd-desktop-reloaded/) - Vermaden builds a new AMD desktop on FreeBSD, and documents the part-picking pain.
* [**M2: Episode 1 (or, Asahi Linux on M3)**](https://www.reddit.com/r/AsahiLinux/s/08wnsWiVZq) - Asahi Linux progress notes on the M3.

## Homelab, Networking & SDR

* [**MOS**](https://mos-official.net/) - A Devuan-based, modular OS for servers and homelabs: web UI for storage and shares, users, Docker, LXC, VMs and monitoring, with no telemetry.
* [**Homelable**](https://homelable.net/) - Self-hosted visual canvas to map, document and monitor a homelab, now also available as a Home Assistant integration via HACS.
* [**gnacho/netpulse**](https://github.com/gnacho/netpulse) - Read-only PWA dashboard for OpenWrt and GL.iNet fleets: per-router health, devices, WireGuard peers and AdGuard Home stats.
* [**Please consider running a NTP server in the NTP Pool**](https://dreamstation.systems/personal/ntppool.html) - Demand for pool capacity keeps growing; here is what running a server involves.
* [**Yet Another LuCI for OpenWrt**](https://play.google.com/store/apps/details?id=com.nightcode.luci) - An Android app for managing OpenWrt and GL.iNet routers, with VPN and parental controls.
* [**GNU Radio World**](https://gnuradioworld.com/) - Build and run GNU Radio flowgraphs in the browser, GRC-style, with hundreds of DSP blocks and RTL-SDR support.

## Hardware & Gaming

* [**AMD BC-250 Documentation**](https://elektricm.github.io/amd-bc250-docs/) / [**The "$60 Gaming PC" - AMD BC-250**](https://devquasar.com/hardware/the-60-gaming-pc-amd-bc-250/) - Community docs for the ex-console board, plus a write-up on turning it into a cheap Linux gaming machine.
* [**DS5_Bridge**](https://github.com/SundayMoments/DS5_Bridge) / [**DS5Dongle**](https://github.com/awalol/DS5Dongle) - Two Pico 2 W projects that turn a Raspberry Pi board into a wireless DualSense dongle.
* [**Cosmos Update - No Man's Sky**](https://www.nomanssky.com/cosmos-update/) - Space stations, galactic alliances and hull salvage to haul back from deep space.
* [**Play GTA Vice City in the browser**](https://quenq.com/apps/vice-city-online/) - A WebAssembly port of the full game, with saves and controller support.
* [**danielbrendel/krepagotchi-game**](https://github.com/danielbrendel/krepagotchi-game) - A pixelated virtual pet game.

## Security & Privacy

* [**LG smart TVs caught logging audio with screen off**](https://www.notebookcheck.net/LG-smart-TVs-caught-logging-audio-with-screen-off-and-snooping-on-local-devices.1391214.0.html) - A Gamers Nexus investigation found the sets sweeping local networks to map nearby devices and capturing microphone audio, uploaded once back online.
* [**Tell HN: OpenAI keeps re-enabling the "allow training" setting**](https://news.ycombinator.com/item?id=49643556) - Users report the setting flipping back on after being switched off.

## Development, Web & Misc

* [**Slifronic/magic-tree**](https://github.com/Slifronic/magic-tree/tree/main) - An isometric 3D tree whose plot is a scannable QR code, built with React and three.js.
* [**What do Visa and Mastercard do?**](https://tautology.town/2026/06/01/card-networks.html) - An intro to card networks and where the money actually moves.
* [**It took a year to ship WebAssembly in Anubis**](https://anubis.techaro.lol/blog/2026/anubis-wasm/) - The long road to a WASM proof-of-work challenge, compiler bug and RAM-starved build machine included.
* [**Music theory for programmers**](https://runjs.app/blog/music-theory-for-programmers) - Notes, scales and chords derived from scratch in JavaScript, with code you can hear.
* [**Don't Let Anyone Take Away Your Big Box of Cables**](https://blog.jim-nielsen.com/2026/hands-off-my-cables/) - A defence of keeping the physical spares around.
* [**Automattic CEO Matt Mullenweg put on leave of absence**](https://www.404media.co/wordpress-automattic-ceo-matt-mullenweg-put-on-leave-of-absence/) - The board voted to put the WordPress co-founder on leave; he says members conspired behind his back.
* [**Michael Jackson's style and Bob Fosse's Snake**](https://www.reddit.com/r/interestingasfuck/comments/1w8zmd6/michael_jacksons_iconic_style_fashion_and/) - The week's off-topic link: the Little Prince number behind the choreography.
