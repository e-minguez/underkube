---
title: "What Edu is reading this week (March 23 - April 5, 2026)"
date: 2026-04-05T08:00:00+02:00
draft: false
slug: 2026-04-05-what-edu-is-reading-this-week-mar-23-apr-05-2026
aliases:
  - /posts/2026-04-05-what-edu-is-reading-this-week-mar-23-apr-05-2026/
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
  - asahi
  - supply-chain
---

After a refreshing week off on PTO, I'm back with a double-sized edition covering two weeks of interesting finds in the tech world. This update features a heavy focus on the emerging "NanoClaw" ecosystem, several critical supply chain security disclosures, and some fascinating hardware hacks.

## Cloud, Kubernetes & Infrastructure

* [**7 Configuration Changes That Turn a Multi-Homed Host Into a Switch/Router**](https://patrickmccanna.net/7-configuration-changes-that-turn-a-multi-homed-host-into-a-switch-router/) / [**How to turn anything into a router**](https://nbailey.ca/post/router/) - Educational deep dives into transforming standard Linux hosts and PCs into functional home routers.
* [**uHTTPd Web Server Configuration**](https://openwrt.org/docs/guide-user/services/webserver/uhttpd) - Detailed guide for configuring the default OpenWrt web server through UCI.
* [**helm-exporter**](https://github.com/sstarcher/helm-exporter) - A Prometheus exporter that provides metrics for Helm releases, charts, and versions running within a Kubernetes cluster.
* [**TopoLVM**](https://github.com/topolvm/topolvm/) - A capacity-aware CSI plugin for Kubernetes that utilizes LVM to provide local persistent storage with dynamic provisioning.
* [**kaito-project/airunway**](https://github.com/kaito-project/airunway) - A Kubernetes-native platform that provides a unified CRD to simplify the deployment and management of LLMs.
* [**The Complete Guide to Self-Hosting: Building Your Personal Cloud Empire**](https://thecybersecguru.com/tutorials/self-hosting-guide/) - A comprehensive tutorial covering hardware, software, and security fundamentals for a private cloud ecosystem.
* [**My Home Network Observes Bedtime with OpenBSD and PF**](https://ratfactor.com/openbsd/pf-gateway-bedtime) - A guide on using OpenBSD and the PF packet filter to automate an internet "bedtime" schedule for specific devices.
* [**dmachard/CoreDNS-GSLB**](https://github.com/dmachard/CoreDNS-GSLB) / [**DNS-collector**](https://github.com/dmachard/DNS-collector) - Powerful tools for Global Server Load Balancing and high-performance DNS data capture and processing.
* [**Project NOMAD**](https://www.projectnomad.us/) - An open-source offline server project providing access to knowledge resources like Wikipedia and local AI without an internet connection.
* [**Drop-in Binary Replacement: Migrate from MinIO to RustFS**](https://rustfs.dev/binary-replacement-a-simple-way-to-migrate-from-minio-to-rustfs/?ref=selfh.st) - A guide on migrating from archived MinIO versions to RustFS via direct binary replacement.
* [**Who Owns Home Assistant, and What Are Commercial Partners?**](https://apolloautomation.com/blogs/news/who-owns-home-assistant-the-open-home-foundation-nabu-casa-and-apollo-automation-explained?ref=selfh.st) - An explanation of the governance structure of Home Assistant under the Open Home Foundation.

## AI, Agents & Tools

* [**NanoClaw**](https://nanoclaw.dev/) / [**Docker Sandboxes**](https://nanoclaw.dev/blog/nanoclaw-docker-sandboxes) / [**The Story Behind the Deal**](https://techcrunch.com/2026/03/13/the-wild-six-weeks-for-nanoclaws-creator-that-led-to-a-deal-with-docker/?ref=selfh.st) - The rapid rise of NanoClaw, a secure, lightweight AI agent runtime that recently secured a major partnership with Docker.
* [**Anthropic restricting Claude subscriptions for OpenClaw**](https://news.ycombinator.com/item?id=47633396) / [**Claude Code Unpacked**](https://ccunpacked.dev/) / [**Anatomy of the .claude/ Folder**](https://blog.dailydoseofds.com/p/anatomy-of-the-claude-folder) - A collection of insights into Anthropic's new CLI agent, including its internal structure and evolving subscription policies.
* [**Guinndex**](https://guinndex.ai/) - A platform dedicated to sharing and contributing to AI-related datasets.
* [**Fine-tuning LLMs Guide**](https://unsloth.ai/docs/get-started/fine-tuning-llms-guide) - A comprehensive technical guide by Unsloth on efficient model fine-tuning methods like LoRA and QLoRA.
* [**ONLYBOTS.store**](https://www.onlybots.store/) - A unique digital storefront designed specifically for AI agents to purchase digital art using autonomous payments.
* [**KV Caching Explained: Optimizing Transformer Inference Efficiency**](https://huggingface.co/blog/not-lain/kv-caching#standard-inference-and-the-rise-of-kv-caching) - An educational blog post explaining how KV caching speeds up text generation in AI models.
* [**AmElmo/proofshot**](https://github.com/AmElmo/proofshot) / [**ProofShot Landing Page**](https://proofshot.argil.io/) - CLI tools and services that allow AI coding agents to verify their work via browser recordings and logs.
* [**alvinreal/awesome-openclaw-tips**](https://github.com/alvinunreal/awesome-openclaw-tips) - A curated collection of tips and configurations for improving the reliability and integration of OpenClaw agents.
* [**Is the Future of AI Local?**](https://tombedor.dev/open-source-models/) - An exploration of why open-source models running on local hardware may dominate due to performance parity and rising cloud costs.
* [**danveloper/flash-moe**](https://github.com/danveloper/flash-moe) - A high-performance inference engine for running massive Mixture-of-Experts models on a laptop by streaming weights from SSD.
* [**aimux**](https://github.com/zanetworker/aimux) - TUI dashboard for managing AI coding agent sessions (Claude, Codex, Gemini)
* [**llamastack/llama-stack**](https://github.com/llamastack/llama-stack) - Composable building blocks to build LLM Apps

## Linux & Systems

* [**asahi-fairydust-display**](https://github.com/bharambetejas/asahi-fairydust-display) / [**Bazzite PR**](https://github.com/ublue-os/bazzite/pull/2155#issuecomment-4154199926) / [**Kernel Compile Guide**](https://blog.clf3.org/post/asahi-kernel-compile/) - Essential tools and guides for the Apple Silicon Linux ecosystem, from USB-C display support to custom kernel building.
* [**Debunking Zswap and Zram Myths**](https://chrisdown.name/2026/03/24/zswap-vs-zram-when-to-use-what.html) / [**Hacker News Discussion**](https://news.ycombinator.com/item?id=47500746) - Kernel engineer Chris Down and the community dive into why zswap is generally superior for most Linux memory management scenarios.
* [**Cocoa-Way**](https://github.com/J-x-Z/cocoa-way?tab=readme-ov-file) - A native macOS Wayland compositor written in Rust for running Linux applications seamlessly on macOS.
* [**The Forge is Our New Home**](https://communityblog.fedoraproject.org/the-forge-is-our-new-home/) - Fedora Project announces the launch of Fedora Forge, a new Forgejo-powered platform for internal code.
* [**Moving from GitHub to Codeberg, for Lazy People**](https://unterwaditzer.net/2025/codeberg.html) - A practical guide for migrating projects to Codeberg and leveraging Forgejo Actions.
* [**Running Tesla Model 3's Computer on My Desk**](https://bugs.xdavidhu.me/tesla/2026/03/23/running-tesla-model-3s-computer-on-my-desk-using-parts-from-crashed-cars/) - Salvaging and powering a Tesla MCU on a desk to explore its software and hardware for bug hunting.
* [**Wine 11 Rewrites How Linux Runs Windows Games at the Kernel Level**](https://www.xda-developers.com/wine-11-rewrites-linux-runs-windows-games-speed-gains/) - Performance gains in Wine 11 driven by the new NTSYNC kernel driver and WoW64 overhaul.
* [**[opensuse-factory] reproducible builds status 2026-02**](https://lists.opensuse.org/archives/list/factory@lists.opensuse.org/thread/QH2ULPPQD5U54TEK5OMWLUEFWSGMLIS5/) - Monthly update on the progress and status of reproducible builds within the openSUSE Factory repository.
* [**MaXX Interactive Desktop**](https://docs.maxxinteractive.com/) - A modern re-implementation of the classic SGI IRIX Interactive Desktop for Linux and FreeBSD.
* [**CURL > /DEV/SDA**](https://astrid.tech/2026/03/24/0/curl-to-dev-sda/) - Exploring the "shitpost" premise of installing Linux by piping a disk image directly to a block device.

## Development, Web & Tools

* [**How a Poisoned Security Scanner Backdoored LiteLLM**](https://snyk.io/de/articles/poisoned-security-scanner-backdooring-litellm/) / [**Attack Transcript**](https://futuresearch.ai/blog/litellm-attack-transcript) / [**Supply Chain Analysis**](https://futuresearch.ai/blog/litellm-pypi-supply-chain-attack/) - A deep dive into the recent LiteLLM supply chain attack, from initial compromise to automated response.
* [**Package Managers Need to Cool Down**](https://simonwillison.net/2026/Mar/24/package-managers-need-to-cool-down/#atom-everything) / [**Resolution - uv**](https://docs.astral.sh/uv/concepts/resolution/#dependency-cooldowns) - Discussing "dependency cooldowns" as a security practice to allow time for community verification of package updates.
* [**Canary Tokens at Grafana Labs**](https://grafana.com/blog/canary-tokens-learn-all-about-the-unsung-heroes-of-security-at-grafana-labs/) / [**Bitcoin Canary in .bashrc**](https://x.com/i/status/2036531640676262187) - Digital tripwires for security detection, ranging from enterprise-scale tokens to @johnloeber's clever BTC-based burglar alarm.
* [**Open Source Index**](https://insights.linuxfoundation.org/open-source-index/) / [**OSSInsight**](https://ossinsight.io/) / [**Repo Health**](https://repo-health.up.railway.app/) / [**Open Source Has a Bot Problem**](https://glama.ai/blog/2026-03-19-open-source-has-a-bot-problem?ref=selfh.st) - Tools and discussions focused on measuring project health and managing the surge of AI-generated contributions.
* [**The Comforting Lie of SHA Pinning**](https://www.vaines.org/posts/2026-03-24-the-comforting-lie-of-sha-pinning/) - A security analysis demonstrating how GitHub Actions' reliance on commit SHAs for dependency pinning can be exploited.
* [**Decompiling the White House App**](https://blog.thereallo.dev/blog/decompiling-the-white-house-app) - A security deep-dive uncovering invasive tracking, paywall bypass scripts, and supply chain risks in the official app.
* [**Change your Google Account username**](https://blog.google/products-and-platforms/products/workspace/google-account-username-change/?ref=selfh.st) - Google now allows U.S. users to change their Gmail username while maintaining their account.
* [**Thaw**](https://github.com/stonerl/Thaw) - A macOS menu bar management utility for organizing and hiding menu bar items.
* [**Microsoft Clarity**](https://clarity.microsoft.com/) - A free user behavior analytics tool offering session recordings and heatmaps.
* [**interview-company-wise-problems**](https://github.com/liquidslr/interview-company-wise-problems) - Curated lists of LeetCode interview questions organized by company frequency.
* [**legalize-es**](https://github.com/EnriqueLop/legalize-es) - Consolidated Spanish legislation in Markdown format, versioned with Git to track reforms.
* [**Shell Tricks That Actually Make Life Easier**](https://blog.hofstede.it/shell-tricks-that-actually-make-life-easier-and-save-your-sanity/) - Practical terminal shortcuts and commands for improved productivity.
* [**The Logfile Navigator**](https://lnav.org/) - Advanced terminal-based log viewer with merging, searching, and filtering capabilities.
* [**Magic Link Pitfalls**](https://etodd.io/2026/03/22/magic-link-pitfalls/) - Analysis of security and UX pitfalls in magic link authentication systems.
* [**richardg867/WaybackProxy**](https://github.com/richardg867/WaybackProxy) - A retro-friendly proxy serving archived web pages without modern scripts for vintage browsers.
* [**The Slow Collapse of MkDocs**](https://fpgmaas.com/blog/collapse-of-mkdocs/) - An account of maintainership issues leading to the fragmentation of the MkDocs project.

## Gaming, Fun & Misc

* [**Dial-up revisited (FOSDEM)**](https://fosdem.org/2026/schedule/event/UJKT3L-dial-up-howto/) / [**Build your own dial-up ISP**](https://www.jeffgeerling.com/blog/2026/build-your-own-dial-up-isp-with-a-raspberry-pi/) - Hardware and software stacks for running a personal dial-up ISP to connect legacy hardware to the modern web.
* [**resumex/doom-over-dns**](https://github.com/resumex/doom-over-dns) / [**Can It Resolve Doom?**](https://blog.rice.is/post/doom-over-dns/) - Compressing DOOM into 2,000 DNS TXT records to run the game engine entirely over the DNS protocol.
* [**Artemis II crew halfway to Moon**](https://www.bbc.com/news/articles/ce8jzr423p9o) - NASA's Artemis II mission captures spectacular high-resolution images of Earth on its lunar journey.
* [**Broadband Magnetic Loop for the MiniRadio**](https://peterneufeld.wordpress.com/2026/03/16/broadband-magnetic-loop-for-the-miniradio/) - Design and construction of a portable magnetic loop antenna for high-performance radio reception.
* [**Apple Discontinues the Mac Pro**](https://9to5mac.com/2026/03/26/apple-discontinues-the-mac-pro/) - Apple retires the Mac Pro line, signaling a shift toward the Mac Studio for pro users.
* [**SLAPMAC**](https://slapmac.com/) - A humorous app that uses the MacBook's accelerometer to make the laptop "scream" when physically slapped.
* [**Obsolete Sounds**](https://citiesandmemory.com/obsolete-sounds/) - A global project collecting and reimagining disappearing sounds from our technological past.
* [**The Hottest New Phone is Tin Can**](https://www.businessinsider.com/tin-can-landline-kids-cellphone-cell-alternative-how-2025-9) - A WiFi-based "landline" for children designed as a mobile phone alternative with strict parental controls.
* [**25 Hit Songs written by Giorgio Moroder**](https://www.youtube.com/watch?v=zxZOhiG3poM) - A musical journey through the legendary producer's career, from disco classics to iconic movie soundtracks.
