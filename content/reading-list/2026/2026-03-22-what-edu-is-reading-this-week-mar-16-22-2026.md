---
title: "What Edu is reading this week (March 16 - 22, 2026)"
date: 2026-03-21T09:00:00+01:00
draft: false
slug: 2026-03-22-what-edu-is-reading-this-week-mar-16-22-2026
aliases:
  - /posts/2026-03-22-what-edu-is-reading-this-week-mar-16-22-2026/
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
  - openwrt
  - btrfs
---

A diverse week featuring deep dives into Btrfs scaling, a flurry of new AI agent control planes, and some critical security updates for CI/CD pipelines.

## Cloud, Kubernetes & Infrastructure

* [**FOSDEM 2026 - The Filesystem Diaries: Scaling Btrfs in an Enterprise**](https://fosdem.org/2026/schedule/event/YVK8KP-scaling-btrfs-in-an-enterprise/) - A detailed look at the challenges and solutions for employing Btrfs at scale in large organizational environments.
* [**Scaling Btrfs to petabytes in production: a 74% cost reduction story**](https://thenewstack.io/btrfs-petabyte-cost-reduction/) - How one team managed to slash infrastructure costs by leveraging Btrfs features for massive data storage.
* [**VictoriaMetrics: Creating the best remote storage for Prometheus**](https://faun.pub/victoriametrics-creating-the-best-remote-storage-for-prometheus-5d92d66787ac) - (2018) - A comprehensive guide on using VictoriaMetrics as a high-performance, cost-effective remote storage backend.
* [**Starlink on OpenWrt 25.x: IPv6, MSS Clamp Fix, BBR and fq_codel**](https://forum.openwrt.org/t/starlink-on-openwrt-25-x-ipv6-mss-clamp-fix-bbr-and-fq-codel-optimisation-guide/247685) - A must-read guide for optimizing Starlink performance on the latest OpenWrt versions.
* [**kimspect**](https://github.com/koithos/kimspect) - A handy kubectl utility to help you quickly inspect container images directly on your pods and nodes.
* [**Fake GPU Operator**](https://docs.nvidia.com/cloud-functions/current/latest/fake-gpu-operator.html) - NVIDIA's development tool for testing GPU-dependent workloads without requiring physical GPU hardware.
* [**QoSmate**](https://github.com/hudra0/qosmate) - Advanced Quality of Service management for OpenWrt, offering granular control over latency and traffic.
* [**Geomate**](https://github.com/hudra0/geomate) - A geographic game server filter for OpenWrt that lets you control your connection zones via a map interface.
* [**diegobernardes/openwrt**](https://github.com/diegobernardes/openwrt) - An Ansible-based project for configuring the NanoPi R6S as a high-performance OpenWrt router.

## AI, Agents & Tools

* [**ClawRemove**](https://github.com/tianrking/ClawRemove) - A specialized CLI tool to audit and clean up the runtime environments of various AI agents like OpenClaw and Cursor.
* [**Unsloth Studio**](https://unsloth.ai/docs/new/studio) - The new interface for fine-tuning LLMs with Unsloth, making model optimization more accessible.
* [**zeroboot**](https://github.com/adammiribyan/zeroboot) - Sub-millisecond VM sandboxing for AI agents, leveraging copy-on-write forking for rapid deployment.
* [**OpenSquirrel**](https://github.com/Infatoshi/OpenSquirrel) - A native Rust/GPUI control plane designed to run Claude Code, Codex, and Cursor side by side.
* [**hiclaw**](https://github.com/alibaba/hiclaw) - An open-source collaborative multi-agent OS that focuses on human-in-the-loop task coordination.
* [**CoPaw**](https://github.com/agentscope-ai/CoPaw) - An easy-to-install personal AI assistant with extensible capabilities supporting multiple chat platforms.
* [**NemoClaw**](https://github.com/NVIDIA/NemoClaw) - A secure environment for running OpenClaw inside NVIDIA OpenShell with managed inference.
* [**tandem-browser**](https://github.com/hydro13/tandem-browser) - An experimental "symbiotic" browser where humans and AI agents can navigate the web as a single entity.
* [**pixel-agents**](https://github.com/pablodelucca/pixel-agents) - A charming pixel-art office environment designed specifically for hosting and monitoring AI agents.
* [**Forge**](https://mistral.ai/news/forge) - Mistral AI's latest toolset for building and deploying high-performance AI models.
* [**ClawLibrary**](https://github.com/shengyu-meng/ClawLibrary) - A 2D pixel-game-style library interface for browsing and monitoring OpenClaw's activity and assets.
* [**A Visual Introduction to Machine Learning**](https://r2d3.us/visual-intro-to-machine-learning-part-1/) - A beautifully animated, high-signal explanation of core machine learning concepts.
* [**Niantic & AI Training Controversy**](https://x.com/S0N_IA/status/2033313278202363985): Serious questions raised about Niantic using Pokémon GO player data to train autonomous delivery robots.

## Linux & Systems

* [**Framework founder Nirav reviews Apple Neo vs Framework Laptop 12**](https://youtube.com/watch?v=uvYt1GgcsUI) - A fascinating comparative teardown and review of the latest hardware designs.
* [**Our commitment to Windows quality**](https://blogs.windows.com/windows-insider/2026/03/20/our-commitment-to-windows-quality/) - Microsoft's latest update on their efforts to improve system stability for Windows Insiders.
* [**Trivy Under Attack: GitHub Actions Compromise**](https://socket.dev/blog/trivy-under-attack-again-github-actions-compromise) - A critical security report on how attackers force-updated tags to deliver malware through CI/CD pipelines.
* [**Bringing Chrome to ARM64 Linux Devices**](https://blog.chromium.org/2026/03/bringing-chrome-to-arm64-linux-devices.html) - Google officially announces that Chrome is finally coming to ARM64 Linux in Q2 2026.
* [**How Kernel Anti-Cheats Work**](https://s4dbrd.github.io/posts/how-kernel-anti-cheats-work/) - A deep dive into the technical mechanisms modern games use for protection at the kernel level.
* [**nvidia_greenboost**](https://gitlab.com/IsolatedOctopi/nvidia_greenboost) - A clever kernel module that transparently extends NVIDIA VRAM by utilizing system RAM and NVMe storage.
* [**SELinux: Finding an elegant solution for gaming on Tumbleweed**](https://security.opensuse.org/2025/06/06/selinux-gaming.html) - Managing security policies while maintaining a smooth experience for emulated Windows gaming.
* [**Android Kernel Tutorials**](https://github.com/ravindu644/Android-Kernel-Tutorials) - A comprehensive starting point for anyone looking to learn the ropes of Android kernel development.
* [**Duranium: A more reliable postmarketOS**](https://postmarketos.org/blog/2026/03/17/introducing-duranium/) - Introducing a new sub-project aimed at significantly improving the reliability of postmarketOS.
* [**Tin Can Linux**](https://tincan-linux.github.io/) - A minimal Linux distribution project focused on simplicity and core system understanding.
* [**openSUSE: Community refines Git packaging workflow**](https://news.opensuse.org/2026/02/19/community-refines-git-packaging-workflow/) - Improving the developer experience for packaging software using modern git-based flows.

## Development, Web & Tools

* [**shipper**](https://gitlab.com/esr/shipper) - Eric S. Raymond's automated tool for shipping open-source project releases across multiple platforms.
* [**Chromebrew**](https://chromebrew.github.io/) - The go-to package manager for ChromeOS users who want more flexibility without using Crouton.
* [**Repology**](https://repology.org/) - An essential service for tracking and comparing package versions across hundreds of different repositories.
* [**sshsrv**](https://github.com/Crosse/sshsrv) - A tool that allows you to connect to SSH servers by leveraging DNS SRV records for service discovery.
* [**Using the Compose Key**](https://crescentro.se/posts/compose-key/) - A quick guide on how to efficiently type special characters on Linux using a designated compose key.
* [**Face Recognition for Bticino Intercoms**](https://github.com/fmanicone/face_recognition_bticino_100x-300x) - Integrating modern face recognition capabilities into classic home intercom systems.
* [**HaleHound-CYD**](https://github.com/JesseCHale/HaleHound-CYD) - An offensive security toolkit ported to the ESP32-based "Cheap Yellow Display."

## Gaming, Fun & Misc

* [**Making A Giant Zipper To Explain How It Works**](https://www.youtube.com/watch?v=9szhjhO9epA) - A mechanical deep dive into the surprisingly complex world of the common zipper.
* [**Surface-Stable Fractal Dithering Explained**](https://youtube.com/watch?v=HPqGaIMVuLs) - A technical explanation of graphics dithering techniques that remain stable across surfaces.
* [**picoCAD 2 Basics in 5 minutes**](https://youtube.com/watch?v=ejpmTDYOBmI) - Getting started with the latest version of the popular low-poly 3D modeling tool.
* [**theflow0 ported Linux to the PS5**](https://x.com/i/status/2030011206040256841) - Security researcher Andy Nguyen's ported Linux to the PS5 and turned it into a Steam Machine. Running GTA 5 Enhanced with Ray Tracing.
* [**maclock**](https://github.com/fensoft/maclock) - A fun project retrofitting an ESP32 and LCD into a classic Macintosh enclosure.
