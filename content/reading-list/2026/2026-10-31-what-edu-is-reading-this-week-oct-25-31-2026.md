---
title: "What Edu is reading this week (Oct 25 - 31, 2026)"
date: 2026-10-31T07:00:00+01:00
draft: false
slug: 2026-10-31-what-edu-is-reading-this-week-oct-25-31-2026
aliases:
  - /posts/2026-10-31-what-edu-is-reading-this-week-oct-25-31-2026/
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
  - hardware
  - sdr
  - gaming
---

A security heavy week: a backdoor inside the official Claude Code extension bundle on the Cursor Marketplace, a 16 year old bug in the EDK2 PXE driver, four Tailscale SSH bulletins and six ZDI kernel reports without a CVE. Around that, Gemini 4 Carbon, speech models in Ollama and a good batch of handheld, radio and smart home material.

## Supply Chain and Certificate Trust

* [**Official Claude Code Extension Compromise**](https://phorion.io/blog/offical-claude-code-vsx-compromise/) - Phorion found a backdoor in the official Claude Code for VS Code bundle on the Cursor Marketplace that sets up a persistent SSH backdoor on macOS, Linux and Windows; affected versions are 2.1.312 and 2.1.313, which Cursor's own notice now names, and the write-up walks through the macOS persistence.
* [**Apple's git still trusts the compromised eMudhra certificates**](https://emudhra.we-have-a-problem.com/apple.html) / [**Apple Support: about the compromised eMudhra intermediate CAs**](https://support.apple.com/en-us/149555) - Eleven days after Apple was notified on 17 October, the git, curl and python3 that ship with macOS still accepted the compromised intermediates, and macOS 27.2 undid the workaround admins had applied by hand. The page includes a git ls-remote check against a test repo; Apple's note says Safari, Mail and the frameworks have blocked the certificates since 19 October and explains how to stop the command line tools trusting /etc/ssl/cert.pem early.

## Kernel, Firmware and Advisories

* [**Tailscale SSH: investigation update**](https://tailscale.com/ssh-investigation-update) - Most of the Tailscale SSH findings are privilege escalation: someone already authorised to connect may be able to act beyond their configured local user. Four bulletins (TS-2026-014 to TS-2026-017) and a follow-up post, with TS_SSH_DISABLE_FORWARDING=1 named as the mitigation while patching.
* [**Code-execution flaw in UEFI firmware affects most servers on planet Earth**](https://arstechnica.com/security/2026/10/code-execution-flaw-in-uefi-firmware-threatens-most-servers-on-planet-earth/) - CVE-2026-97631, a 16 year old buffer overflow in the EDK2 PXE Base Code driver: an ICMP error longer than the 504 byte field is copied past it, so a packet sent during network boot runs code in ring 0 and can reach the TPM, which breaks disk encryption if the attacker can touch the network. Ars explains why the public AMI pull request moved the disclosure forward.
* [**Detecting and mitigating ZDI-CAN-33367 and five other Linux flaws**](https://www.sysdig.com/blog/detecting-and-mitigating-zdi-can-33367-and-five-other-linux-flaws) - The six reports ZDI sent in October, one in ConnMan and five in the kernel, none with a CVE yet and two at CVSS 9.0. A public root exploit for ZDI-CAN-33367 works on current Ubuntu, Debian and AlmaLinux, and this post ranks the batch and gives detection and mitigation per distribution.
* [**cups local privilege escalation**](https://x.com/apiratemoo/status/2113836338906603666) / [**cowcups PoC**](https://codeberg.org/piratemoo/cowcups) - Local root through libcupsfilters 2 to 2.2.1: the PoC chains cups-browsed, libcupsfilters and ghostscript (with -i include path) to get code execution as root from a privileged printing service, using remotely advertised printer discovery.

## AI, Agents and Models

* [**Gemini 4 Carbon: our next frontier model**](https://blog.google/innovation-and-ai/models-and-research/gemini-models/introducing-gemini-4-carbon/) - Google's new frontier model leads the Artificial Analysis Intelligence Index v5.0 at 59, with SEC-bench Pro at 88.2 percent, ExploitGym at 54.8 and CWE-bench at 71.0, plus 89 elo more on WebDev Arena. Same introductory price as Argon ($2 and $10 per million tokens), rolled out to cyber defenders first through the Fairwind Program.
* [**Speech models in Ollama**](https://ollama.com/blog/speech-models) - Ollama 0.40.11 can read text aloud with Phonon from Gradium: five languages, dozens of voices, streamed as it is generated, macOS only for now, and about 35 percent faster than Gradium's own runtime on an M5 Max.
* [**Niko1221/Strata**](https://github.com/niko1221/strata) / [**Running Qwen 3.8 Flash Next on 8 GB of VRAM**](https://www.reddit.com/r/LocalLLaMA/comments/1xft2ae/have_8_gb_of_vram_and_32_gb_of_ram_you_can_run/) - Strata is a one click installer and inference engine for Qwen3.8-Flash-Next, the 125B MoE, on 8 GB or more of NVIDIA memory, exposing an OpenAI and Anthropic compatible API on localhost with optional image input. The thread reports about 900 t/s prompt processing and 30 t/s generation on that hardware.

## Linux, Kernels and Desktops

* [**scx_horoscope**](https://github.com/zampierilucas/scx_horoscope) / [**sched-ext/scx**](https://github.com/sched-ext/scx) - A sched_ext scheduler that makes real decisions from planetary positions: fire signs boost CPU tasks 1.5x, retrograde motion applies a 50 percent slice penalty, a full moon lifts interactive tasks 1.4x, and it genuinely loads into the kernel through scx_rustland_core. The upstream tree is the serious version of the same idea, with schedulers written in BPF that load and unload at runtime.
* [**Ghostty 1.4.0 release notes**](https://ghostty.org/docs/install/release-notes/1-4-0) - Released 27 October after seven months: large performance and memory improvements, a complete Kitty graphics implementation with animation and relative placements (the first terminal outside Kitty), SSH integration work, and 2,889 commits from 172 contributors.
* [**AlpineBSD wiki**](https://wiki.alpinebsd.org/) - An operating system on the NetBSD kernel with a userspace inspired by Alpine Linux (apk-tools, busybox, GNU leanings) and an explicit goal of shipping as little AI generated code as possible, with an AI policy covering the base system and the main repository. No installer yet.
* [**Simple NetBSD webserver**](https://bsandro.tech/posts/simple-netbsd-webserver/) - bsandro's recipe for a small NetBSD 11 server with bozohttpd and one extra package for HTTPS, from a VPS with a preloaded image, aimed at small sites rather than heavy traffic.

## Homelab, Self-Hosting and Smart Home

* [**Kestrel User Guide**](https://www.3ntropy.io/kestrel-user-guide/) - The manual for Kestrel 1.0.10 (stable on 30 October), a headless Wi-Fi handshake capture device: staging the SD card before first boot, a Bluetooth phone tether or Wi-Fi for management, the browser dashboard, the capture whitelist, plugins for temperature, session stats, GPS and the UPS HATs, and a learning agent that picks between a baseline and four capture algorithms.
* [**HACS is now the Home Assistant Marketplace**](https://frenck.dev/hacs-is-now-the-home-assistant-marketplace/) - From Home Assistant 2026.11, HACS ships inside Home Assistant as the Marketplace under Settings, with custom integrations, dashboard cards and themes migrating automatically. Franck Nijhof on the rename, what stays the same and why nothing costs money.
* [**BTicino-GO-Integration**](https://github.com/abeilprincipino/BTicino-GO-Integration) - A Home Assistant custom integration and Lovelace card for a rooted BTicino Classe 300X or 100X running GO Companion: local push over the companion's /api/v3 API, intercom camera as an entity, ring on an incoming call, and answer, talk, hang up and unlock from a dashboard.
* [**lenovo-smart-clock-linux**](https://github.com/kortregt/lenovo-smart-clock-linux) - Replacing Android Things with Alpine Linux on the Lenovo Smart Clock gen 1 (CD-24501F, sparrow): AVB unlock, full eMMC backup with mtkclient, a kernel built from Google's source, Wi-Fi, audio, a plain framebuffer display and an LVGL clock face, all done from a Mac with one USB-A to USB-A cable and no soldering. The target use is Home Assistant.
* [**rommapp/romm**](https://github.com/rommapp/romm) - A self-hosted ROM manager and player: scans and enriches a collection from more than ten metadata providers, browses and plays in the browser with EmulatorJS and RuffleRS, syncs saves across devices and covers over 400 platforms.
* [**Duck DNS**](https://www.duckdns.org/) / [**Port Forward**](https://portforward.com/) / [**intoDNS for duckdns.org**](https://www.intodns.com/duckdns.org) - The pieces for reaching a home server from outside: Duck DNS for a free dynamic DNS name hosted on AWS, portforward.com for the per router steps to open a port, and intoDNS to check a domain's parent records, glue, nameservers and mail setup.
* [**Phantomdrive**](https://rootkitlabs.com/phantomdrive/) / [**o7-machinehum/phantomdrive**](https://github.com/o7-machinehum/phantomdrive) - An open source USB drive that presents 8 GB of normal storage and hides the rest behind an unlock file containing password:yourpassword, from which an AES-XTS key is derived; storage is an SD card, the SoC is a CH569W, and hardware, firmware and enclosure files are all published.

## Handhelds and Consoles

* [**ALVA-Store/MyShell**](https://github.com/ALVA-Store/MyShell) - A PS5 inspired homebrew launcher for the PS Vita, now 1.1.0: a full library view separate from the short home carousel, uninstall from inside the launcher, background music in beta, PS1 to PS4 anniversary themes and SteamGridDB artwork.
* [**vita-turbo-storage**](https://github.com/juanjsebgarcia/vita-turbo-storage) - A taiHEN kernel plugin for firmware 3.60 to 3.74 that removes the cache cleaning and invalidation around every storage read, about 40 percent of the time of each read on an SD2Vita, by handing the system driver a buffer that needs no cache work. Early release, tested on a single PCH-1000.
* [**CrankBoy v3.0.0**](https://github.com/CrankBoyHQ/crankboy-app/releases/tag/v3.0.0) - The Playdate Game Boy emulator gets roughly 40 percent faster emulation, voice sample support, 30/50/60 frame modes, a Cover Flow library view, editable categories built from the ROM database genres, HuC1 and HuC3 mappers, MBC7 accelerometer support, and a half translated Japanese UI.
* [**TG4PD**](https://highlyintegratedgayhijink.itch.io/tg4pd) - An unofficial Telegram client that runs on the Playdate itself, with no phone tether and no bridge server: Telegram's encrypted protocol on the device over Wi-Fi, QR login, chats, folders, reactions, 1-bit photos, voice notes you crank through, polls and bot buttons.
* [**My experience daily driving a PS5 with Linux as a desktop PC**](https://www.reddit.com/r/PS5_Jailbreak/comments/1xhzuwu/my_experience_daily_driving_a_ps5_with_linux_as_a/) - Someone using a jailbroken PS5 with Linux as their main desktop because their own PC (an i5 6400 and an RTX 2060 that has since become a GTX 1650) is dated.
* [**PS5 14.10 Jailbreak Tracker**](https://ps5-jb-tracker.vercel.app/en) - One page tracking the four public firmware 14.10 research projects (ZigZagBoi1, pastawithpesto, kuzibelit and zecoxao) with last commit times and summaries, and a plain warning that none of them is a working jailbreak.
* [**piermark/omarchytv**](https://github.com/piermark/omarchytv) - An Omarchy styled tiling launcher that runs on Android TV, Google TV, LG webOS, Android phones and Linux, macOS or Omarchy desktops from the same ecosystem.

## SDR, Radio and Hardware

* [**FalconSDR**](https://github.com/rafafunt/FalconSDR) / [**browser demo**](https://falconsdr.com/) / [**SoapySDR wiki**](https://github.com/pothosware/SoapySDR/wiki) - A wideband scanner that only records real transmissions, with a browser UI for a local or headless receiver, a searchable library and optional Whisper transcription, over RTL-SDR or SoapySDR. The demo runs the real interface against a simulated receiver, and the wiki explains the vendor neutral abstraction layer behind the SoapySDR path.
* [**ATS Mini Controller**](https://atsminiradio.com/en) / [**games for the ATS Mini**](https://www.reddit.com/r/ATSminiRadio/s/0Q4AhAJYLs) - A free browser remote for the ATS Mini (ESP32-S3 and SI4732) shortwave receiver over Web Serial or Web Bluetooth: tuning, scanning, memory slots, screenshots, and a firmware installer that detects the official, Monster or Berndt build. A community thread shows small games written for the radio.
* [**ats-mini-monster**](https://github.com/Ho52198/ats-mini-monster) - A fork of the ATS Mini firmware with encoder shortcuts (hold and rotate for direct frequency entry), direct access to volume, squelch, step, bandwidth and AGC from the info panel with deferred confirmation for band and mode, and a rebuilt three column dark web interface with battery readout.
* [**Raspberry Pi Zero 3 W and Pi 4 Model A on the Way?**](https://bret.dk/raspberry-pi-zero-3-w-pi-4-model-a/) - Device tree files in the kernel tree point to a Zero 3 W using the Pi 4's BCM2711 and to a cut down Pi 4 Model A. Bret reads the names and what the hardware would imply.

## Retro, Gaming and Fun

* [**RecompLauncher**](https://recomplauncher.com/) - A launcher and store for recompiled console games on PC: it installs and updates native builds and ships no game files, you bring your own disc. The catalogue runs from Ship of Harkinian and Zelda 64 to SpaghettiKart, Starship and Banjo: Recompiled.
* [**Zelda Oracles Combined**](https://www.romhacking.net/hacks/10150/) / [**ROM generator**](https://soaresden.github.io/ZeldaOracleCombinedFR/) - Oracle of Ages and Oracle of Seasons merged into a single Game Boy Color ROM, switchable from Vasu's shop with one inventory, in five languages. The browser generator builds it from your own European ROMs on the US disassembly, sends nothing anywhere, and can also build the two games separately.
* [**encarta_95_web**](https://github.com/benwinding/encarta_95_web) - Microsoft Encarta 95 running entirely in the browser through v86: a pre-booted Windows 95 snapshot loads straight into Encarta, with the hard disk and the CD streamed on demand, a pointer lock mode for desktop and a touch model for phones.
* [**Guías Nintendo 2000**](https://archive.org/details/guias_nintendo_2000) - A preservation archive of the guides Nintendo España published on its website in the late nineties and early 2000s, kept in their original layout.
* [**Bronco Release**](https://www.patreon.com/zelbrad/posts/bronco-release-173372027) - A mod release that swaps a car body for a full four door Ford Bronco, with sharp panel lines and working headlights, tail and brake lights. Posted on Patreon.
* [**TitleArt**](https://titleart.dvy.io/) - Every classic WordArt style, shape and 3-D effect from 1997, back in the browser.
* [**Shitty Screenshare**](https://shittyscreenshare.com/) - A small site arguing for WHIP: OBS and FFmpeg can publish straight into a video conference over WebRTC with a server URL and a bearer token, so you choose resolution, bitrate and codec instead of letting the browser pick.
* [**Firefox reunites meme royalty to ask what happened to the web**](https://blog.mozilla.org/en/firefox/come-back-to-firefox/) - Mozilla brings back Overly Attached Girlfriend, Dancing Matt and Annoying Orange to argue that the early web was yours, and that forced AI features are more annoying than any of them.
