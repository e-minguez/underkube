---
title: "What Edu is reading this week (Aug 2 - Sep 5, 2026)"
date: 2026-09-05T09:00:00+02:00
draft: false
slug: 2026-09-05-what-edu-is-reading-this-week-aug-2-sep-5-2026
aliases:
  - /posts/2026-09-05-what-edu-is-reading-this-week-aug-2-sep-5-2026/
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
  - gaming
---

Back from holidays, so this one covers everything that piled up over the last month: new model releases, Slurm on Kubernetes, a lot of BSD, the Omarchy funding argument, ADS-B receivers and a stack of retro and homelab projects.

## AI, Models & Agents

* [**Introducing Claude Fable 5.1 and Claude Mythos 5.1**](https://www.anthropic.com/claude-fable-and-mythos-5-1): Anthropic's latest models for coding and knowledge work, with an early look at how they contribute to scientific research.
* [**Introducing Gemini 3.8 Flash and 3.8 Flash Cyber**](https://blog.google/innovation-and-ai/models-and-research/gemini-models/3-8-flash-and-3-8-flash-cyber/): Google's next Flash generation, with a variant aimed specifically at agentic cybersecurity workflows.
* [**Qwen3.8-Max: A New Bar for Coding and Cowork**](https://news.ycombinator.com/item?id=49150470) / [**Qwen Studio**](https://qwen.ai/blog?id=qwen3.8): The Qwen 3.8 release and the studio around it — chat, image and video understanding, generation, document processing, search and tools — plus the Hacker News discussion.
* [**Ox Alpha**](https://oxalpha.com/) / [**Bloomberg coverage**](https://unwall.app/www.bloomberg.com/news/articles/2026-08-26/china-s-z-ai-made-ox-alpha-stealth-model-that-rivals-deepseek): A stealth reasoning model with a 1M-token context window, free and login-free, reportedly built by China's Z-ai.
* [**Nvidia agrees to buy Hugging Face for $12.9 billion**](https://www.reuters.com/technology/nvidia-talks-acquire-hugging-face-13-billion-deal-business-insider-reports-2026-08-27/): Reuters on the reported acquisition.
* [**The right open model for every use case**](https://helmcode.com/open-model-guide): 82 enterprise use cases mapped to the open-weight model that solves each one, verified as of 1 September 2026.
* [**Why your local LLM feels dumber than it is**](https://forum.level1techs.com/t/why-your-local-llm-feels-dumber-than-it-is/253917): A long, technical series of experiments on how quantisation and implementation-specific hazards make local inference diverge from the reference implementation.
* [**llmman**](https://llmmanorg.github.io/): Manage and serve LLM models as standard OCI artifacts — Ollama-, OpenAI- and Anthropic-compatible APIs from one small binary.
* [**NVIDIA-NeMo/Switchyard**](https://github.com/NVIDIA-NeMo/Switchyard): Route LLM traffic across models and providers while keeping native OpenAI and Anthropic API compatibility, for benchmarking and cost/performance tuning.
* [**leonickson1/Swiftlet**](https://github.com/leonickson1/Swiftlet): A Swift and Metal runtime that streams expert weights from storage so 35B and 80B Qwen MoE models run locally on Apple devices, iPhones included.
* [**Mem0**](https://mem0.ai/) / [**Self-hosted setup**](https://docs.mem0.ai/open-source/setup): A memory layer that lets agents keep learning from past interactions, with a REST server, dashboard, API keys and audit log you can run yourself.
* [**Garry Tan's company brain**](https://github.com/garrytan/gbrain/blob/master/docs/tutorials/company-brain.md): An opinionated tutorial for building an agent "brain" over a company's own material.
* [**What is a Harness?**](https://earendil.com/posts/what-is-a-harness/): A clear definition of the agent harness — the software that provides the environment a model operates within.
* [**Claude system prompts release notes**](https://platform.claude.com/docs/en/release-notes/system-prompts): Anthropic publishes the changes to the core system prompts behind claude.ai and the mobile apps.
* [**Boost deep reasoning (/boost)**](https://antigravity.google/docs/boost/): Google Antigravity's slash command for pushing tricky bugs and algorithmic problems through multi-agent reasoning loops.
* [**Graphify-Labs/graphify**](https://github.com/Graphify-Labs/graphify): An agent skill that turns any folder — code, SQL schemas, R and shell scripts, docs, papers, images, video — into a queryable knowledge graph.
* [**AminBlg/SimpleEnglish**](https://github.com/AminBlg/SimpleEnglish) / [**mge1512/skill-claudism-pass**](https://github.com/mge1512/skill-claudism-pass): Two writing skills — one makes LLMs write docs in ASD-STE100 Simplified Technical English, the other scrubs AI-writing tells and adapts drafts for an international technical readership.
* [**Spec Kitty**](https://spec-kitty.ai/): A delivery control plane that turns local agent work into reviewable progress — specs, work packages, evidence, reviews and launch readiness in one record.
* [**Don't be a meat proxy**](https://gruhn.me/blog/2026-08-03/): Relaying AI output verbatim adds nothing; read it, validate it, and rewrite it in your own words.
* [**Is AI Profitable Yet?**](https://isaiprofitable.com/): A single-purpose site answering exactly the question in its name.
* [**fal.live**](https://fal.live/) / [**Building a brand on the fal.ai agent**](https://x.com/lenxism/article/2091993265486590265): A continuous AI-generated broadcast where viewers decide what happens next, and the write-up of a product and brand built from scratch on the same platform.
* [**ElevenLabs, TwelveLabs, ThirteenLabs, …**](https://quantumi.sh/public/labs.html): Cataloguing the AI industry's number-plus-"labs" naming convention from 0 to 99.
* [**VibeCoded AI-Slop License v1.0**](https://gist.github.com/NicolasCARPi/3fd349ed1ed52ae6b835d5364cda4cd6): A licence text for the current moment.

## Cloud, Kubernetes & HPC

* [**Slinky**](https://slurm.schedmd.com/slinky.html) / [**SlinkyProject/slurm-operator**](https://github.com/SlinkyProject/slurm-operator) / [**nebius/soperator**](https://github.com/nebius/soperator): SchedMD's own project for running Slurm on Kubernetes, its operator, and Nebius' alternative operator for the same job.
* [**Slurm Quick Start User Guide**](https://slurm.schedmd.com/quickstart.html) / [**Slurm Lab**](https://gitlab.com/CSniper/slurm-lab) / [**ClusterdOS**](https://gitlab.com/aranya-tech/public/clusterdos): The official primer plus a hands-on lab and a cluster OS project to practise against.
* [**NCP-AII Training & Practice Lab**](https://www.dclabsim.com/): Free prep for the NVIDIA AI Infrastructure certification — 229 simulated datacenter commands, guided scenarios and practice exams.
* [**Metal3 Meets KubeVirtBMC: Provisioning KubeVirt VMs Like Bare Metal**](https://blog.zespre.com/metal3-meets-kubevirtbmc/): An end-to-end demo of Metal3 provisioning KubeVirt VMs through virtual BMC endpoints, exactly as if they were physical servers.
* [**From Ingress to Gateway API: How We Modernized Networking on Our GKE Cluster**](https://the-devops-engineer.medium.com/from-ingress-to-gateway-api-how-we-modernized-networking-on-our-gke-cluster-8409ffb53173): A production migration from the traditional Ingress controller to the Gateway API.
* [**We Blamed CoreDNS for Weeks. The Real Culprit Was a Default We Never Questioned**](https://medium.com/@a.warkhade98/the-issue-159436266391): A DNS resolution mystery in a microservices cluster that turned out not to be CoreDNS at all.
* [**selvarajmurugesan90/klarity**](https://github.com/selvarajmurugesan90/klarity): A read-only, GitOps-first Kubernetes observability dashboard with auto-discovery and native ArgoCD/Flux integration.
* [**spinningfactory/kloak**](https://github.com/spinningfactory/kloak): Cloud-native zero trust security for AI agent run environments.
* [**Apple Container v1.2.2**](https://x.com/i/status/2086079142898909186): The release adds the ability to create a standalone Kubernetes cluster you manage with kubeadm.
* [**How I Rebuilt YouTube's Load Balancing Algorithm in Go**](https://medium.com/@sathwick.p7/how-i-rebuilt-youtubes-load-balancing-algorithm-in-go-9a8ea8b39c8f): Why the obvious guess about distributing traffic across millions of backends is wrong.

## Linux & Desktop

* [**CERN Transitioning Industrial Computers To Debian**](https://www.phoronix.com/news/CERN-Goes-Debian-Leaving-RHEL): A longtime RHEL/CentOS institution moves its industrial control machines to Debian.
* [**Linus Torvalds Endures A Debug Session From Hell, "Enormously Helped" By AI**](https://www.phoronix.com/news/Linus-Torvalds-Debug-AI): Torvalds authors an Intel Xe graphics driver patch himself, with an unusual credit.
* [**Doubly linked list**](https://0xax.dev/books/linux-inside/linux-datastructures-1): The linux-inside chapter on the kernel's most-used data structure.
* [**cpunoise v0.2**](https://lore.kernel.org/all/20260815083728.15470-1-marco.crivellari@suse.com/T/): Announcement of a CPU isolation testing tool on the kernel list.
* [**Support of XBOOTLDR in openSUSE**](https://news.opensuse.org/2026/07/07/xbootldr/): More boot partition space for BLS setups under systemd-boot and GRUB2-BLS.
* [**openSUSE/berghain**](https://github.com/openSUSE/berghain/): An openSUSE-branded fork of Berghain, the Go and HAProxy "bouncer" that validates browsers before letting them reach a backend.
* [**EasyEffects should be part of every Linux distribution**](https://www.osnews.com/story/145883/easyeffects-should-be-part-of-every-linux-distribution-and-desktop-environment-to-massively-improve-laptop-speaker-sound-quality/) / [**Easy Effects Manual**](https://wwmm.github.io/easyeffects/): The case for shipping EasyEffects by default to fix laptop speaker sound, plus the manual to do it yourself.
* [**OpenLogi**](https://openlogi.org/en): A native, local-first alternative to Logitech Options+ written in Rust — remap buttons, drive DPI and SmartShift over HID++, no account, no telemetry.
* [**dharmx/walls**](https://github.com/dharmx/walls): A large, well-curated wallpaper repository.
* [**10-year-old bug action triggered an Ubuntu Phone dev reunion**](https://www.omgubuntu.co.uk/2026/08/ubuntu-phone-bug-reunion): Closing an ancient Launchpad bug as invalid brought back most of the engineers who worked on it.
* [**Refund4Freedom**](https://en.refund4freedom.org/): Getting a refund for the proprietary operating system licence you never wanted.
* [**Haiku R1/beta6 Release Notes**](https://www.haiku-os.org/get-haiku/r1beta6/release-notes/): What changed in the latest Haiku beta.

## Omarchy

* [**Omacom Foundation launches with $8 million**](https://omarchy.org/news/2026/08/omacom-foundation-launches-with-8-million/) / [**Normalized Fascism in Open Source: $12 Million Given to DHH**](https://brennan.day/normalized-fascism-in-open-source-12-million-given-to-dhh/): The foundation announcement, and a sharply critical response arguing the funding and the politics around it should not be treated as apolitical.
* [**Merchants of Insecurity**](https://blog.happyfellow.dev/merchants-of-insecurity/): A blunt security review of what Omarchy 4.0 shipped, and why the author recommends against it.
* [**Omarchy Web**](https://omarchy.nkz.md/) / [**Omarchy Demo**](https://omarchy-demo.org/): Two ways to try Omarchy in a browser tab before installing — boot the machine, work the menu, try the themes.
* [**aorumbayev/awesome-omarchy**](https://github.com/aorumbayev/awesome-omarchy): A curated list of Omarchy resources.
* [**astrofoundry/omarchy-keybind-editor**](https://github.com/astrofoundry/omarchy-keybind-editor): An editor for Omarchy keybindings.
* [**aorumbayev/deckarchy**](https://github.com/aorumbayev/deckarchy): Fix Steam Deck OLED hardware issues after installing Omarchy on vanilla Arch.
* [**omarchy-mac**](https://github.com/omarchy-mac/omarchy-mac) / [**ggalancs/omarchy-arm-utm**](https://github.com/ggalancs/omarchy-arm-utm) / [**maralcbr/omarchy-mx-mac**](https://github.com/maralcbr/omarchy-mx-mac): Three routes to Omarchy on Apple Silicon — an opinionated Arch/Hyprland setup for M1/M2, a native aarch64 UTM VM built from macOS by one script, and experimental compatibility through Arch Linux ARM and Asahi.
* [**TouchID working on Omarchy**](https://x.com/0xBOYD/status/2092616493787730294?s=20): TouchID on a 2016-17 T1 TouchBar MacBook, apparently a Linux first.

## BSD

* [**BSDnas**](https://bsdnas.com/) / [**FreeCORE**](https://freecore.org/): Two community forks carrying TrueNAS CORE forward on FreeBSD after its discontinuation.
* [**Code That Built the Internet: The Impact of BSD, Part 2**](https://www.lpi.org/blog/2026/06/26/code-that-built-the-internet-the-impact-of-bsd-part-2/): From sendmail to containers, the conclusion of LPI's series on BSD's lasting influence.
* [**httpd.rocks**](https://httpd.rocks/) / [**bozohttpd rocks**](https://bozo.httpd.rocks/): Setting up an HTTPS-enabled web server with httpd on OpenBSD, and the same idea with bozohttpd on NetBSD.
* [**Run OpenBSD on DigitalOcean for $4/month**](https://nil.wallyjones.com/run-openbsd-on-digitalocean-for-4month/) / [**Migrating from Codeberg Pages to an OpenBSD VPS**](https://nemin.hu/vps/index.html): Two practical accounts of putting a small site on OpenBSD.
* [**NetBSD and my life...**](https://mail-index.netbsd.org/netbsd-advocacy/2005/09/10/0000.html): A 2005 netbsd-advocacy post worth the click.

## Apple Silicon & Mac

* [**Progress Report: Linux 7.2**](https://asahilinux.org/2026/08/progress-report-7-2/): The latest on porting Linux to Apple Silicon.
* [**Dissecting the Apple M1 GPU, the end**](https://alyssarosenzweig.ca/blog/asahi-gpu-part-n.html): Alyssa Rosenzweig closes out the M1 GPU reverse-engineering series.
* [**KAIT2EN Fedora**](https://kait2en.org/) / [**project page**](https://kait2en.github.io/): Cutting-edge T2 Mac support on stock Fedora — kernels from Fedora, T2 modules via DKMS.
* [**Apple's new desktop computers are designed specifically for local AI development**](https://arstechnica.com/apple/2026/08/with-new-mac-studio-and-mac-mini-apple-leans-hard-into-local-ai-inference/): The Mac Studio and Mac mini refresh leans into local inference and Mac daisy-chaining.
* [**An (updated) guide to 6W idle consumption on MacBook Pro 13" Early 2015**](https://www.reddit.com/r/linux_on_mac/s/xtxkg49Apj): Tuning an old MacBook to 6W idle on Fedora 44.
* [**angristan/MacThrottle**](https://github.com/angristan/MacThrottle): A menu bar app that tells you when your Mac is thermal throttling.
* [**hjanuschka/shitty-shortcuts**](https://github.com/hjanuschka/shitty-shortcuts): Bind a cheap macro keypad to Lua scripts with a Hammerspoon-compatible API, no accessibility permissions needed.
* [**Apple's hidden white noise feature**](https://www.fastcompany.com/91272739/apple-mac-background-sound-white-noise-focus-productivity-mac-os-ventura): Background Sounds, buried in macOS, as a focus tool.
* [**osx360/osx360-drivers**](https://github.com/osx360/osx360-drivers): Xbox 360 controller kernel extensions for Mac OS X.

## Self-Hosting & Homelab

* [**dockur/windows**](https://github.com/dockur/windows): Windows inside a Docker container.
* [**Unmanic**](https://github.com/Unmanic/unmanic): A library optimiser that keeps a media collection in the formats you actually want.
* [**NicolasGoeddel/zfs-snapshot-explorer**](https://github.com/NicolasGoeddel/zfs-snapshot-explorer): A simple file explorer for ZFS snapshots.
* [**Monitoring SystemD services with Healthchecks.io**](https://passbe.com/2022/healthchecks-io-systemd-checks/) / [**official docs**](https://healthchecks.io/docs/monitoring_systemd_tasks/) / [**discussion**](https://lobste.rs/s/dxfl0r/monitoring_systemd_services_with): Using systemd's OnSuccess and OnFailure hooks to ping Healthchecks.io, with the docs and the Lobsters thread.
* [**my server is a phone now**](https://seg6.space/posts/phone-server/): Rooting a CMF Phone 1 to run personal infrastructure at home.
* [**An E-Ink Homelab Dashboard on a Jailbroken Kindle**](https://mxd.codes/articles/an-e-ink-homelab-dashboard-on-a-jailbroken-kindle): Why the Kindle renders nothing itself, and why half the first draft of the dashboard got deleted.
* [**How I Turned My Security Cameras Into an Automatic Bird Identification System with BirdNet-Go**](https://jasontucker.blog/how-i-turned-my-security-cameras-into-an-automatic-bird-identification-system-with-birdnet-go/): Three security cameras repurposed into real-time bird species tracking.
* [**europaprof/call14**](https://github.com/europaprof/call14): A $20 local-first smart elevator call and tracking system built with ESP8266, Home Assistant, MQTT and computer vision.
* [**Javisen/dgt_traffic**](https://github.com/Javisen/dgt_traffic): A Home Assistant integration for real-time geolocated traffic incidents, EV chargers and weather events from Spain's DGT DATEX2 feeds.
* [**HomeCritters**](https://github.com/HomeCritters): Firmware and a Home Assistant integration that turn a round-screen ESP32-S3 into a desk pet — Leon the ferret gets hungry, plays and reacts to local weather, all locally.
* [**andreabenini/keymaker**](https://github.com/andreabenini/keymaker): A two-factor authenticator for the ESP-CYD using OTP protocols.
* [**Create a Phoniebox - Bluetooth Speaker Edition**](https://docs.google.com/document/d/e/2PACX-1vSaPey4ZwUduA6k4vfFbAh1Foxjuu7MuKHZCQwjugnC8ywr78mkIXtCNahYTskuTjAsI1K7aUH1TjEr/pub): Building an RFID audio box for kids, in Bluetooth speaker form.

## Networking

* [**An interactive introduction to the spanning tree protocol**](https://vincent.bernat.ch/en/blog/2026-spanning-tree): Root election, port roles, proposals and agreements, topology changes — RSTP explored through simulations powered by MSTPD compiled to WebAssembly.
* [**Nace XDP DNS**](https://bandaancha.eu/articulos/nace-xdp-dns-servicio-publico-resolucion-11897) / [**Oihalitz/xdp-dns-evadeproxy**](https://github.com/Oihalitz/xdp-dns-evadeproxy): In Spanish — a public resolver hardened against indiscriminate IP blocking, and the Rust DNS proxy that transparently rewrites anycast IPs to get around it.
* [**Movistar y O2 arreglan la lentitud de YouTube**](https://share.google/uXdve5R3TfBk9QhLU): Forum users found the cause of the YouTube slowdown before the ISP did.
* [**routeup**](https://routeup.dev/): Stable HTTPS names for local apps — `example-app.localhost` instead of `localhost:3000`, local by default and public only when you choose.
* [**Pinggy**](https://pinggy.io/docs/): Tunnels for hosting sites, receiving webhooks, sharing files and reaching localhost remotely.
* [**Yet Another LuCI for OpenWrt**](https://play.google.com/store/apps/details?id=com.nightcode.luci): A native Android OpenWrt and GL.iNet router manager with LuCI, ubus, VPN and parental controls.

## Security

* [**tmp.0ut Volume 5**](https://tmpout.sh/5/): The August issue of the ELF and binary research zine — polyglot ELFs, metamorphic viruses, code virtualisation, syscall hooks, extreme size optimisation and an interview with Doug McIlroy.
* [**Amazon kept shutting down my tablet, so I spent $266 on four AI models to own it**](https://ericpardee.github.io/fire-hd-ownership/): Five months, CVE-2022-38181 and four models spent on actually owning a Fire HD.

## Development, Web & Tools

* [**PostgreSQL for Everything**](https://www.raphaelbauer.com/posts/postgresql-everything/): The case that PostgreSQL can replace Kafka, Redis, ClickHouse and Elastic, and the companies already doing it.
* [**The Move to Python 3 Begins!**](https://www.eveonline.com/news/view/the-move-to-python-3-begins): How CCP migrates 2.4 million lines of EVE Online code.
* [**SecretSpec 0.20**](https://secretspec.dev/blog/secretspec-0-20-git-docker-inline-specs-and-five-new-providers/): Git and Docker retrieve credentials from any provider, secrets declared in application code, a JVM SDK and Alpine deployments.
* [**Audacity 4.0.0**](https://github.com/audacity/audacity/releases/tag/Audacity-4.0.0): The interface rebuilt on Qt with a new clip-editing model, keeping most Audacity 3 workflows.
* [**OpenShot 4.0**](https://www.openshot.org/blog/2026/08/30/openshot-40-record-edit-color-like-never-before/): Professional colour grading, screen and webcam recording, local object masks, 10 new effects and a native timeline.
* [**Bear Blog**](https://bearblog.dev/): Free, no-nonsense, very fast blogging.
* [**UnWall**](https://unwall.app/): Paste a URL, get a clean reader without paywalls, consent popups or ads.
* [**nuno-faria/tetris-sql**](https://github.com/nuno-faria/tetris-sql/tree/main): Tetris, built on SQL's Turing completeness.

## SDR & Aviation

* [**ADS-B Reception, Decoding & Sharing with Docker**](https://sdr-enthusiasts.gitbook.io/ads-b): The reference guide for building an ADS-B receiver stack in containers.
* [**docker-adsb-ultrafeeder**](https://github.com/sdr-enthusiasts/docker-adsb-ultrafeeder) / [**docker-planefence**](https://github.com/sdr-enthusiasts/docker-planefence) / [**docker-acarshub**](https://github.com/sdr-enthusiasts/docker-acarshub): An all-in-one ADS-B container with readsb, tar1090, graphs1090, autogain and mlat-hub; a fence that logs the aircraft passing over your house; and an ACARS/VDLM2 receiver.
* [**machineinteractive/skies-adsb**](https://github.com/machineinteractive/skies-adsb): Turn unfiltered ADS-B data from an RTL-SDR into a real-time 3D air traffic display with custom maps.
* [**Overhead Sky**](https://overheadsky.com/): A small Mac menu-bar app naming the aircraft passing overhead — live callsign, type and route.

## Hardware, Retro & Gaming

* [**MartyPC Web Edition**](https://martypc.net/?machine_config_name=ibm5150_xtide&machine_config_overlays=ibm_cga&scaler_preset=IBM+5153): An IBM PC/XT emulator written in Rust, now compiled for the web.
* [**slap**](https://slap.nyuu.page/) / [**project page**](https://nyuu.page/projects/slap/): Apply, create, convert and inspect ROM patches in twenty formats, in the browser or the terminal.
* [**BlackLabelHQ/SymphonyRecomp**](https://github.com/BlackLabelHQ/SymphonyRecomp): A static recompilation project for Castlevania: Symphony of the Night.
* [**Midrags/SFF**](https://github.com/Midrags/SFF): A Steam game setup and management tool covering manifests, Lua integrations, multiplayer fixes and backups.
* [**Game Bundle Guardian**](https://gamebundleguardian.com/bundles?sort=worthiest): Compare Humble, Fanatical and other bundles — guarding your wallet from games you will never install.
* [**Cobalt: apps and an SDK for Kobo e-readers**](https://bandarlabs.github.io/Cobalt/): A launcher, signed app store, Rust SDK and capability-isolated runtime for the Kobo Clara BW.
* [**Xiaomi's new CPU matches Apple on single thread**](https://x.com/lemire/status/2091894299289874926): Daniel Lemire on the new Xiaomi silicon — comparable single-threaded, considerably faster multithreaded.

## Fun & Misc

* [**.name Termination**](https://neil.fraser.name/news/2026/09/03/): ICANN approved Verisign's plan to eliminate third-level `.name` domains, taking down Neil Fraser's site, email and IoT services by February 2027 — and leaving the vacated name for anyone to register.
* [**50,000 boat names**](https://www.beautifulpublicdata.com/boat-names/): A deep dive into AIS vessel data, from SEA SLUT II to BILBOAT BAGGINS.
* [**How does IKEA come up with names for its products?**](https://www.ikea.com/se/en/customer-service/knowledge/articles/6f564c4d-2ccc-46de-b643-545a3948dc79.html): IKEA explains its naming system, which is strange even to Swedish speakers.
* [**Galaxium**](https://galaxium.app/): Fly from Earth to planets, stars, nebulae and distant galaxies in 3D in your browser.
* [**Air Theremin**](https://theremin.bizibah.com/): Play a theremin in mid-air with phone motion or camera hand tracking, with scales, cave reverb and recording.
* [**Halftone QR Codes**](https://cgv.cs.nthu.edu.tw/Projects/Recreational_Graphics/Halftone_QRCodes/) / [**Dithered QR code generator**](https://www.andrewt.net/dithered-qr-codes/wtf/) / [**Color photo QR codes**](https://1mentat.github.io/qr-code-shenanigans/): Three steps up the same ladder — halftone research, a dithered generator you can use, and an extension to full-colour photographs with hue-preserving channel-bound forcing.
* [**Leaked Microsoft pay data**](https://www.businessinsider.com/microsoft-staff-share-pay-in-internal-spreadsheet-see-the-numbers-2026-8): What some Microsoft employees in AI, cloud and other teams are making, from a spreadsheet they shared themselves.
