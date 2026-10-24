---
title: "What Edu is reading this week (Oct 18 - 24, 2026)"
date: 2026-10-24T07:00:00+02:00
draft: false
slug: 2026-10-24-what-edu-is-reading-this-week-oct-18-24-2026
aliases:
  - /posts/2026-10-24-what-edu-is-reading-this-week-oct-18-24-2026/
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
  - php
  - gaming
  - sdr
  - android
  - hardware
---

A week dominated by PHP2Shell: two critical memory safety bugs in core PHP, found with AI assistance, plus the emergency releases and a messy fight over the disclosure. Around it, eMudhra's certificate authority collapse, OpenBSD 8.0 and a good batch of ports, radio and desktop material.

## PHP2Shell and AI-Found Vulnerabilities

* [**PHP2Shell**](https://www.php2shell.com/) - Landing page for the two CVEs in core PHP (out of memory handling and stale global state) reaching CVSS 9.2, with unauthenticated remote code execution, upgrade guidance and the research credited to Wiz, OpenAI Codex Security and Calif.
* [**RCE via OOM corruption**](https://github.com/php/php-src/security/advisories/GHSA-w8hw-w9fx-j79w) / [**RCE via stale global state**](https://github.com/php/php-src/security/advisories/GHSA-6wmf-4rv5-p3rp) - The two php-src advisories: longjmp() on allocation failure leaving request memory in an invalid state, and global state surviving into the next request as a use after free.
* [**Upcoming Critical PHP Security Release**](https://news-web.php.net/php.announce/509) - The php.announce warning published ahead of the fix, with two CVSS 9.2 issues scheduled for release on 21 October at 14:00 UTC.
* [**PHP: News Archive - 2026**](https://www.php.net/archive/2026.php#2026-10-20-1) - The release announcement (8.5.12, 8.4.27, 8.3.36 and 8.2.35) plus a follow-up advisory on session upload progress, CVE-2026-115560, with session.upload_progress.enabled=0 as the mitigation in the meantime.
* [**openai/php2shell-checker**](https://github.com/openai/php2shell-checker) - Small Node tool and two Codex skills that check a PHP version from a site's headers or a local install and answer OK, potentially vulnerable or unknown.
* [**Patch the Planet: global response coordination as agents uncover critical vulnerabilities**](https://openai.com/index/coordinated-disclosure-of-critical-vulnerabilities/) / [**Patch the Planet**](https://patchtheplanet.org/) - OpenAI on the coalition behind the PHP response (Calif, Wiz, Cloudflare, the maintainers, CISA) and a proposed five stage framework for disclosing AI found bugs; the site collects the disclosures and the guidance.
* [**PHP2Shell: buy time with a WAF, then patch the servers**](https://traefik.io/blog/php2shell-buy-time-with-a-waf-then-patch-the-servers) - Traefik's reading of the two flaws: 9.2 on CVSS 4.0, the bug present since PHP 5.4, 69.3% of websites affected, and attack traffic within hours of the release.
* [**PHP blames supply chain security biz Chainguard for putting huge chunks of the web at risk**](https://www.theregister.com/security/2026/10/22/php-blames-supply-chain-security-biz-chainguard-for-putting-huge-chunks-of-the-web-at-risk/5304611) - The dispute after the fact: PHP maintainers accuse Chainguard of publishing ahead of the coordinated date, and its CEO answers that active exploitation changes the deal.

## Certificate Authorities & Trust

* [**eMudhra to Exit global SSL/TLS Certificate Business**](https://emudhra.com/en/press-release/emudhra-to-exit-global-ssl-tls-certificate-business) - The board decided to withdraw from SSL/TLS certificates after the incident, noting the affected CAs were revoked within 14 hours, no end entity certificates had been issued from them, and the line was about 1% of revenue.
* [**Eight Bits of Trust; eMudhra's CA keys cracked in milliseconds**](https://scotthelme.co.uk/eight-bits-of-trust-emudhras-ca-keys-cracked-in-milliseconds/) - Scott Helme recovers the private keys of the eight compromised intermediates from their public certificates, because some of them are single byte values: 4, 56 and 115.
* [**Protecting Firefox users following the compromise of eMudhra intermediate certificates**](https://blog.mozilla.org/security/2026/10/20/protecting-firefox-users-following-the-compromise-of-emudhra-intermediate-certificates/) - Mozilla's timeline: the report at 20:06 UTC on 17 October, OneCRL blocking in under three hours, then Firefox 158.0.1 and NSS 3.131.1 to remove the root.
* [**Farewell, France**](https://quad9.net/news/blog/au-revoir-france/) - Quad9 withdraws its free DNS service from France on 24 November after a court ordered it to block domains in favour of beIN, with the fine reduced from 580,000 euro to 1,000 euro per day.

## Security Advisories & Incidents

* [**GitLab Critical Patch Release: 19.5.1, 19.4.3, 19.3.6, 19.2.9, 19.1.9, 19.0.10, 18.11.13**](https://docs.gitlab.com/releases/patches/patch-release-gitlab-19-5-1-released/) - Critical patch release from 21 October for self managed installs, with GitLab.com and Dedicated already patched; the details of each issue become public 90 days after the fix.
* [**Several Linux Kernel Vulnerabilities Accidentally Posted To Public Kernel Mailing List**](https://www.phoronix.com/news/LKML-New-Trend-Vulnerabilities) - Trend Micro's Zero Day Initiative sent several unpatched kernel reports to LKML instead of the private security list, including a CVSS 9.0 SMB Direct remote code execution bug.
* [**pwn.watch**](https://pwn.watch/) - Live dashboard of open security incidents with CVEs, patch status, fixed versions, advisories and the posts that broke each one, at around 35 live incidents when saved.

## AI, Agents & Models

* [**The rise and fall of Jev hype**](https://blog.alexewerlof.com/p/rise-and-fall-of-jev-eval-hype-vs-llm) - Alex Ewerlöf takes apart the Jev hype cycle, 33 days after its introduction: a cheap general purpose classifier sold as a decision model, and what the episode says about an industry short of real innovation.
* [**MiniMax M3.1 Flash: Redefining Agent Performance and Cost**](https://www.minimax.io/blog/minimax-m31f) - New Flash model aimed at agentic tasks, computer use and coding, with online inference nearly three times faster and usage costs down about 70%.
* [**WorldTUI: I trained a 360M model to pretend to be a terminal**](https://simedw.com/2026/10/21/world-model-terminal/) - A 360M model with no shell or filesystem behind it that predicts how the screen changes, runs vim and tmux, plays snake and usually remembers your earlier commands; the 208 MB demo runs in a WebGPU browser.
* [**Chinese AI Writes Weaker Code for Beijing's Adversaries. We Fixed It. A Qwen3-Coder Case Study**](https://www.hirundo.io/blog/qwen3-coder-vulnerabilities) - Hirundo traces Qwen3-Coder's less secure code to the weights, then removes the model's alignment from them and reports the gap closing.
* [**rply: an inbox for agents that run without you**](https://rply.sh/) / [**joshuaKnauber/rply**](https://github.com/joshuaKnauber/rply) - One inbox between you and agents that run on servers: updates, questions you answer from the phone, pinned live status and secrets that go straight into a file, with Claude Code, Codex and Hermes on the list.
* [**Tokibot**](https://tokibot.lottes.dev/) / [**a-lottes/tokibot**](https://github.com/a-lottes/tokibot) - E-ink critter on a Pi Zero that shows what your coding agents are up to (working, waiting for permission, rate limited) and eats the tokens they burn; about 50 to 60 euro in parts and no soldering.
* [**How are you managing your Hermes agents from your phone?**](https://www.reddit.com/r/hermesagent/comments/1xavwj1/how_are_you_managing_your_hermes_agents_from_your/) - r/hermesagent thread asking how people drive their Hermes agents remotely, after finding phone side management still clunky when away from the desk.

## Linux & Desktop

* [**OpenBSD 8.0**](https://www.openbsd.org/80.html) - Released 20 October: the amd64 kernel virtual address space raised from 4G to 512G, hibernate on arm64, swap encryption using AES instructions, and a release song called The Simps on AI.
* [**OpenBSD 8.0 | Hacker News**](https://news.ycombinator.com/item?id=50160494) - 158 comments of OpenBSD appreciation: pf, pledge and unveil, man pages that are consistently good, and boxes that serve as bastion hosts and then never need attention.
* [**'emulators/wine' - MARC**](https://marc.info/?l=openbsd-ports&m=179236125692175) - A Wine port proposal for OpenBSD after a software workaround for the %gs issue, with dozens of 64 bit Windows programs tested, the Witcher 3 remaster running with vkd3d-proton, and no WoW64 yet.
* [**Caelestia**](https://caelestiashell.com/) / [**caelestia-dots/caelestia**](https://github.com/caelestia-dots/caelestia) - A fluid, morphing desktop shell and dotfiles set built on Quickshell with the Hyprland config now in Lua, installed through a CLI, plus an unofficial live image in progress.
* [**Hitesh754/omarchy-caelestia**](https://github.com/Hitesh754/omarchy-caelestia) - Brings the Caelestia shell to an Omarchy install while keeping Omarchy's system, Hyprland configuration and applications: Omarchy stays the system layer, Caelestia the visual one through Quickshell.
* [**plusky/halloween-openSUSE**](https://github.com/plusky/halloween-openSUSE) - Cosy autumn Halloween theme for openSUSE Tumbleweed across Plasma, GNOME, Xfce and Sway, with wallpapers, icons, login screens, boot splash, a Firefox theme and a chameleon in a witch hat.
* [**jordanhubbard/daemonarchy**](https://github.com/jordanhubbard/daemonarchy) - Omarchy on FreeBSD: a bootable 16.0-CURRENT image whose installer asks the same questions as the Omarchy ISO, then installs the Hyprland desktop from the x11-wm/omarchy port.

## Cloud, Kubernetes & Networking

* [**Pangolin 1.25: Redirects, mTLS, and Machine Roles**](https://pangolin.net/news/1-25-release) - Adds HTTP redirects with path rewriting, mutual TLS on public resources, roles for machine clients, configurable load balancing strategies, blueprint export and credential regeneration on Community Edition.
* [**Unser PullSecret Operator: ein alltägliches Kubernetes-Problem, sauber gelöst**](https://www.itdpk.de/blog/pullsecret-operator-kubernetes) / [**itdpk-de/pullsecret-operator**](https://github.com/itdpk-de/pullsecret-operator) - A small MIT operator that defines an image pull secret once as a ClusterPullSecret and materialises it into namespaces on demand, with optional registry login validation and a mutating webhook.

## Development & Web

* [**jeetrex17/TDrive**](https://github.com/jeetrex17/TDrive) - Go and Wails desktop file manager that uses a private Telegram channel as the drive, with media streaming, encrypted photo and video backup, shared drives and a scriptable CLI.
* [**weball**](https://www.funwithcomputervision.com/weball/) - Small browser toy where you roll a ball over a page to grow it, with levels and the option to roll up any website you like (pages that build everything client side come out sparse).
* [**Google Rust Style Guide**](https://google.github.io/styleguide/rustguide.html) - Google's rules for Rust code: prefer small crates, avoid Rc and Arc in favour of borrows, accept flexible references, prefer enums over bools in APIs, and keep glob imports out.

## Cars, Radio & Hardware

* [**skuep/Mobile-Whip**](https://github.com/skuep/Mobile-Whip) - Active receive only HF antenna (100 kHz to 30 MHz) based on the Mini-Whip, reworked for a single lithium cell or 5V USB, with a lithium charger, an LTC6268 opamp, 20 mA draw and a 3D printed 200 mm enclosure.
* [**Changelog - ATS Mini documentation**](https://esp32-si4732.github.io/ats-mini/changelog.html) - Firmware 2.45 for the ATS Mini receiver adds an RDS OFF option and fixes missing, truncated or mixed RDS text and station name resets; 2.44 added display, radio, power and connectivity settings to the web config page and moved the Audio Clamp option there.
* [**All-Radio-Tools**](https://github.com/ToftMalone/All-Radio-Tools) - Android app in Kotlin that gathers Wi-Fi, Bluetooth, mobile network and GNSS tools plus HackRF radios for ADS-B, AIS, ACARS, radiosondes, Meshtastic and weather satellites, with no ads or tracking.
* [**Flipper One**](https://flipper.net/pages/flipper-one) - Open Linux device on an RK3576 with a mainline kernel and no binary blobs, Wi-Fi 6E, Gigabit Ethernet and M.2 expansion for 5G or SDR; the early preorder batch is already closed.
* [**OBD-II support for every car**](https://pelican.clutch.engineering/cars) - Pelican's catalog of which makes and models it works with and which OBD-II parameters each one reports, built on the OBDb, the open database of the manufacturer specific commands that J1979 does not cover.

## Decompilations, Ports & Gaming

* [**jailbreaking the switch 2**](https://pepsipu.com/blog/2026-10-switch2-jailbreak-ns2jb/) / [**pepsipu on X**](https://x.com/pepsipu/status/2113117920373137622) - ns2jb, a software only tethered jailbreak for Switch 2 firmware 23.0.1 that runs native code as a sysmodule and as the built-in fs, enough for homebrew, save backups and a Codex modded Mario Kart World.
* [**The Best Way to Play Super Mario 64: on Apple Vision Pro**](https://www.pagetable.com/303) / [**mist64/diorama64**](https://github.com/mist64/diorama64) - Super Mario 64 as an augmented reality diorama on visionOS: each level sits on your real table, you walk around it as the camera and play with a controller, built on sm64coopdx with a Metal renderer.
* [**Doom on a DVD player**](https://blazelight.dev/blog/vobdoom) - Doom's E1M1 on a 75 dollar JVC DVD player from a plain burned DVD-R: the engine runs before the burn, the game rules become DVD navigation code, and the disc holds around 200,000 pre-rendered cells.
* [**BlackLineInteractive/Driveclub-Port**](https://github.com/BlackLineInteractive/Driveclub-Port) - Native port of Driveclub from PS4 to macOS on Metal 3 and to Windows on Vulkan with FSR 4.1.1 and frame generation; the repository is archived now.
* [**PS5 Portal high bitrate: LXC and Docker deployment**](https://github.com/atameric/ps5-portal-high-bitrate/blob/main/deploy%2FREADME.md) - How to run the project's automatic Remote Play relay in a Proxmox LXC or a macvlan Docker container, since the ARP redirection needs its own MAC on the same layer 2 LAN as the PS5 and the Portal.
* [**EarthNG 0.4.0: drive a real place in BeamNG, first native release**](https://www.reddit.com/r/BeamNG/comments/1x9d0hg/earthng_040_drive_a_real_place_in_beamng_first/) - First public build of EarthNG, a BeamNG Lua mod that builds roads, buildings, terrain and vegetation from OpenStreetMap and elevation data as you drive, with no companion server.
* [**RetroCrisis/Retro-Crisis-GDV-NTSC**](https://github.com/RetroCrisis/Retro-Crisis-GDV-NTSC) - Retro Crisis libretro CRT shader presets built on the Guest Advanced NTSC shader, with 720p, 1080p and 4K presets plus install guides for Windows, iOS, Linux and Steam Deck.
* [**otisabiburada/decky-screen-mirror**](https://github.com/otisabiburada/decky-screen-mirror) - Decky Loader plugin that mirrors an iPhone into a picture in picture window over the game in Gaming Mode over AirPlay, with its own receiver, optional PIN approval per phone and a slider for the phone audio only.

## Android & TV

* [**An ad-free Android TV**](https://cretezy.com/2026/ad-free-android-tv) - Replacing the Google TV launcher with Projectivy, YouTube with SmartTube, the Jellyfin client with Wholphin and remapping the remote's YouTube button with Button Mapper, tested on two Chromecasts and a Hisense TV.

## Fun & Misc

* [**First look at LEGO Daft Punk**](https://www.reddit.com/r/DaftPunk/comments/1xcjl1s/first_look_at_lego_daft_punk/) - r/DaftPunk thread with a first look at the LEGO Daft Punk set, 675 points and 40 comments at the time of saving.
