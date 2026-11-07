---
title: "What Edu is reading this week (Nov 1 - 7, 2026)"
date: 2026-11-07T07:00:00+01:00
draft: false
slug: 2026-11-07-what-edu-is-reading-this-week-nov-1-7-2026
aliases:
  - /posts/2026-11-07-what-edu-is-reading-this-week-nov-1-7-2026/
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
  - homelab
  - hardware
  - android
  - gaming
---

A week of releases and one proper security scare: openSUSE Leap 16.1 folds the immutable server edition into Leap itself, NetBSD ships the first point release of the 11 branch, Nvidia publishes a Kubernetes management plane for GPU clusters on bare metal, and OpenSSH races out 10.6p2 for a password bypass on Alpine that was already being exploited under nine hours later. Around them, GPT-6 Cyber turning up 81 unknown Firefox flaws, a car head unit jailbroken just to change the clock and a look at what hardcoded timeouts cost on a slow connection.

## Cloud, Kubernetes and Infrastructure

* [**NVIDIA Kubernetes Engine (NVKE)**](https://github.com/dsx-ai-factory/nvke) / [**HN discussion**](https://news.ycombinator.com/item?id=50387738) - Nvidia open sourced the management plane platform teams install to offer managed Kubernetes on their own GPU hardware: each workload cluster gets its own control plane, etcd and node pools, and NICo is the only infrastructure provider supported at preview. The local quickstart simulates machines with Docker, so you can try it without a GPU. The thread (123 points, 27 comments) asks who needs this outside the NVIDIA Cloud Partner programme, and a commenter describes the target as tenant isolated clusters on the DSX reference stack with hosts wiped and re-attested between tenants.
* [**Bluefin Server 26.11 (Beta)**](https://docs.projectbluefin.io/blog/bluefin-server-beta/) - The server edition is built on Freedesktop SDK libraries, skips bootc and goes pure DDI through BuildStream, and already includes Nvidia and ZFS support. The install menu splits the two use cases it targets: a minimal read only server, or a homelab Kubernetes node with kubeadm, containerd, Argo Workflows and a KubeStellar dashboard, with an option for workers that run diskless with the OS in the UEFI partition.
* [**Mac at any scale**](https://namespace.so/blog/mac-at-any-scale) - What running Macs in a datacenter actually takes: custom MacBook racks, virtualizing macOS with the Apple Virtualization framework, and building and distributing very large VM images across the fleet.

## Linux Distributions

* [**Leap 16.1 Unites Traditional and Immutable Linux in One Release**](https://news.opensuse.org/2026/11/03/leap-unites-traditional-and-immutable/) / [**Release announcement**](https://en.opensuse.org/Release_announcement_16.1) / [**Release notes**](https://doc.opensuse.org/release-notes/x86_64/openSUSE/Leap/16.1/html/release-notes-leap-161/) / [**Upgrade guide**](https://en.opensuse.org/SDB:System_upgrade) - The first minor release of the Leap 16 series absorbs Leap Micro as a new Immutable Mode, so one distribution now covers desktops, servers, container hosts, VMs and edge devices, with the Agama installer and a lifecycle running into the next decade. The release notes list the changes and known issues, and the upgrade guide gives the two supported paths: zypper --releasever 16.1 dup or the opensuse-migration-tool, which also handles Leap to SLES and Tumbleweed moves. Note that Leap 16 needs an x86_64-v2 CPU.
* [**Announcing NetBSD 11.1 (November 2, 2026)**](https://www.netbsd.org/releases/formal-11/NetBSD-11.1.html) - First point release of the 11 branch, focused on security and bug fixes: a boot panic on late model VIA and Zhaoxin CPUs, a NULL dereference in ipfilter while parsing ICMP6 packets, an off by one in the bsd_decompress bounds check, a race in the page daemon, plus sparc64 sensor and i2c work for the Ultra 25/45 and Sun Fire V215/V245.
* [**FOSDEM 2027 BSD, illumos, OpenZFS, bhyve Devroom: call for presentations**](https://people.freebsd.org/~rodrigo/fosdem27/) - The devroom returns on Saturday 30 January 2027, afternoon slot, with FOSDEM itself on 30 and 31 January. Submissions close 7 December 2026 and selected talks are announced on 15 December; slots run 15 to 30 minutes including questions, and everything goes through Pretalx with the BSD track and the Talk event type.

## Desktops and Workstations

* [**Omarchy 4.5**](https://x.com/omarchy/status/2118216477623067099) - The first big release since Quattro adds a traditional desktop mode next to the tiling default, native installs on M1, M2, M3 and Neo MacBooks, and 50 languages. The release notes count 740 pull requests from more than 180 contributors in twelve weeks.
* [**Gershwin**](https://github.com/gershwin-desktop/gershwin-desktop/wiki) - Desktop environment built on GNUstep and aimed at people switching from macOS. The wiki has live ISOs for FreeBSD, Arch, Devuan, Debian and the BSDs, notes that the Devuan image is the one where installation works properly, and warns that Apple machines with a T2 chip need a kernel that is not on the ISOs.
* [**AgenticLinux**](https://agenticlinux.github.io/) - A Fedora 44 desktop image with Claude, Codex, OpenCode, OpenClaw and Goose installed on first boot, next to Docker, Docker Sandboxes and QEMU with KVM and GPU runtimes. The whole OS is a bootc image, so updates are atomic and rollback is one command, and bootc switch moves an existing system to another variant. The ISO is a network installer.

## AI Agents and Tooling

* [**Introducing GPT-6 Cyber**](https://openai.com/index/introducing-gpt-6-cyber/) / [**The Hacker News coverage**](https://thehackernews.com/2026/11/openai-launches-gpt-6-cyber-after-ai.html) - OpenAI's security model, rated Critical under its Preparedness Framework and pitched on alignment as much as capability: it stays inside the scope researchers set in 99.93% of runs (94.49% for GPT-5.6 Cyber) and scores 48.5% on ExploitGym against 32.1% before. With it, researchers found 948 local privilege escalation exploits and 81 previously unknown high severity Firefox flaws that Mozilla is now fixing.
* [**Karpathy says Claude built HackerTube in about two hours**](https://x.com/IntCyberDigest/status/2116997960164913402) - A YouTube front end that only recommends videos Hacker News keeps praising. Claude sifted 43 million comments from 20 years of HN down to 6,454 videos that people kept recommending, and the only manual step was a Google API key.
* [**AI Beacon**](https://github.com/manusa/ai-beacon) - Self hosted Go dashboard for people running several Claude Code or OpenCode sessions across machines. A small CLI on each machine reports its sessions to the dashboard you host, the browser view shows what every agent is doing, it notifies you when one is waiting, and you can type straight into that terminal from a phone. Binaries, the container image and the Helm chart are free during the early access phase, with the source to follow.

## Development and Security

* [**SSHole: an oversized password walks into Alpine (CVE-2026-123158)**](https://www.helpnetsecurity.com/2026/11/06/openssh-sshole-cve-2026-123158-exploitation/) / [**The Hacker News coverage**](https://thehackernews.com/2026/11/hackers-exploited-openssh-sshole-flaw.html) - OpenSSH 10.6p2, out on 5 November, fixes an authentication bypass in sshd on musl Linux without PAM, which is Alpine's default server build: an attacker who can reach the port logs into an account with no password set by sending an oversized password, one connection and no retries. CVSS 8.1, and Previdian's first observed attempt came under nine hours after publication, with confirmed root on a honeypot running real Alpine and OpenSSH. The bug traces back to a 2016 patch for CVE-2016-6210.
* [**Stop Hardcoding Your Timeouts**](https://alfy.blog/2026/04/23/stop-hardcoding-your-timeouts.html) - A rant with a point: unconfigurable timeouts are a tax on everyone outside a fast connection. The npx skills installer chokes on a 30K star skills collection with no flag to raise the limit, the issue has been open since February, and the same pattern shows up in Docker tooling.
* [**Why did you choose the nix you nix?**](https://lobste.rs/s/7fcuxz/why_did_you_choose_nix_you_nix) - Ask thread on which Nix implementation to pick between cppnix, Determinate Nix, Lix and Guix, with 46 comments on the trade offs: the corporate version and its upstreaming habits, Lix fixing papercuts without breaking compatibility, and Guix being a GNU project when you need nonfree software.
* [**PoC Index**](https://pocindex.io/) - Searchable index of public proof of concept exploits built from GitHub, Nuclei, ExploitDB, Metasploit and Vulhub, with CVSS, EPSS and CISA KEV context on each entry. It counts 176,260 CVEs indexed, 85,393 of them with a public PoC, and 1,257 known to be exploited.
* [**I discovered a sound that leaks your exact location**](https://www.youtube.com/watch?v=UytYrhYLOKI) - Combining aircraft ADS-B data with the Doppler curve of a flyover in the spectrogram, a digital elevation model and a 200 metre grid is enough to place a short recording within about 100 metres, in some cases from less than a minute of audio. The video walks through the pipeline and closes with the mitigations.

## Handhelds, Hardware and Self-Hosting

* [**ESP Terminator**](https://espterminator.com/) - Browser based firmware flasher for ESP32 boards, Flipper Zero, Meshtastic, BW16, MonstaTek M1, Marauder, Bruce and M5Launcher, with nothing to install locally.
* [**SKYWRIT**](https://matthewo-0.itch.io/skywrit) - A Playdate game where you steer a murmuration of starlings with the crank. Every bird follows its seven nearest neighbours, so the flock flows around pylons, splits around wind turbines and opens like a curtain when the falcon dives. A sends a ripple through the flock, B calls the stragglers back, and at dusk the birds spell out how many made it home. Three dollars, and the crank also works as a d-pad.
* [**LineageOS 23.2 for Google Kukui (Krane)**](https://github.com/alpha-liu-01/android_device_google_kukui) - Android 16 on the Lenovo IdeaPad Duet, keeping the factory ChromeOS depthcharge bootloader: the image boots from a USB stick with Ctrl+U and an installer copies it to the internal eMMC, either beside an existing Linux install or replacing it. Keyboard, touchscreen, stylus, Wi-Fi, Bluetooth HID, cameras and sensors work and video uses the hardware H.264 decoder, while SELinux stays permissive and external displays are not implemented.
* [**tdt-local**](https://github.com/cibernicola/tdt-local) - Local web viewer for Spanish DTT television and radio fed by the public TDTChannels lists, with guide, multiview and subtitles, plus an optional AI assistant and subtitle pipeline on top of llama.cpp, ffmpeg and whisper.cpp. Only the Python standard library is needed, and the author is upfront that this is a personal project vibecoded with AI.
* [**Memtly**](https://memtly.com/) / [**Memtly.Community**](https://github.com/Memtly/Memtly.Community) - Photo sharing for events: guests open a gallery from a printed QR code, upload what they took, and the host reviews everything before it appears. There are presentation and slideshow modes, audit logs, a pile of settings and a GDPR page, it runs in Docker, Kubernetes or any container host, and the community front end (formerly WeddingShare) is on GitHub.
* [**Disc Image Studio**](https://github.com/JiaFeiMiao-K-Cat/DiscImageStudio/blob/main/README.en.md) - An all in one tool for burning a visible image onto the surface of a CD, DVD or single layer BD-R: it converts a picture into data that respects the physical layer constraints of the disc, so any recorder can etch it and you see the result with the naked eye. Windows GUI plus an experimental CLI for Linux and macOS, .NET 10, GPL 3.0.

## Gaming and Cars

* [**TotK Recomp**](https://github.com/valentderah/totk-pc-recomp) - Static recompilation of Tears of the Kingdom into a native x86-64 application for Windows and Linux with a Vulkan renderer, so no emulation. It takes your own NSP, XCI, NSZ or XCZ dumps, ships no game files, runs at 60 fps by default with up to 144, and carries saves between the 1.2.1 and 1.4.3 updates. Early development: playable, with visual bugs and crashes still expected.
* [**BeamNG protocols**](https://documentation.beamng.com/modding/protocols/) / [**DriveDeck mobile dashboard**](https://www.drivedecks.app/mobile) - BeamNG.drive and BeamNG.tech push telemetry over UDP to external hardware, with OutGauge (the Live For Speed format, so existing dashboards and digital displays already work), other built in protocols and a documented way to write your own. DriveDeck takes the phone route: install the game app plus its companion, start the phone dashboard, scan the QR code, add the page to the home screen and connect with the eight digit code.
* [**Jailbreaking my car to change the time**](https://blog.nns.ee/2026/11/02/renault-hack/) - A 2014 Renault Latitude with a TomTom Carminat LIVE unit that hides the clock setting unless a genuine map SD card is inserted: the menu itself comes from the card, the DRM checks its CID and signed files, and third parties wanted about 60 EUR for one. So he pulled the update image, built a QEMU setup with a 2.6 kernel and a rough CAN emulator, and chained a path traversal in the master.script LOG command with an overwritten core_pattern to get root from a crashing dbus-monitor. The payoff was editing one number in settings.dat, the local offset, from 180 minutes to 120.
