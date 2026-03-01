---
title: "What Edu is reading this week (Feb 23 - Mar 1, 2026)"
date: 2026-03-01T09:00:00+01:00
draft: false
slug: 2026-03-01-what-edu-is-reading-this-week-feb-23-mar-01-2026
aliases:
- /posts/2026-03-01-what-edu-is-reading-this-week-feb-23-mar-01-2026/
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
---

This week's roundup covers a wide range of topics, including the architectural limits of etcd, GPU-initiated networking, the nostalgic design of Apple's breathing lights, and the surprising persistence of floppy disks in transit systems.

![what-edu-is-reading-this-week-feb-23-mar-01-2026](/images/2026-03-01-what-edu-is-reading-this-week-feb-23-mar-01.png)

## Cloud, Kubernetes & Infrastructure

* [**Why etcd breaks at scale in Kubernetes**](https://learnkube.com/etcd-breaks-at-scale) - A deep dive into the architectural limitations of etcd and how hyperscalers are evolving beyond it.
* [**Sympozium (KubeClaw) — Kubernetes-Native Agentic Control Plane**](https://k8sclaw.ai/#architecture) / [**GitHub Repo**](https://github.com/AlexsJones/kubeclaw): A platform for orchestrating AI agents as isolated skill sidecars with ephemeral RBAC.
* [**Scaling AI Document Processing with Ray & KubeRay**](https://medium.com/@gsaisiddharth7/scaling-ai-document-processing-on-kubernetes-with-ray-kuberay-115ff1228501) - Practical patterns for parallelizing GPU-intensive OCR tasks on Kubernetes.
* [**Building NVSHMEM from Scratch: GPU-Initiated Networking**](https://cppcheatsheet.com/notes/blog/nvshmem.html) - An in-depth exploration of RDMA transport and GPUDirect for LLM training.
* [**Configure EFA (Elastic Fabric Adapter) for HPC**](https://oneuptime.com/blog/post/2026-02-12-configure-efa-elastic-fabric-adapter-for-hpc/view) - A guide to low-latency inter-node communication for distributed machine learning.
* [**Amazon EC2 P5 Instances for AI/ML Training**](https://oneuptime.com/blog/post/2026-02-12-use-amazon-ec2-p5-instances-for-aiml-training/view) - Best practices for leveraging H100 GPUs and Flash Attention on AWS.
* [**NVIDIA NCCL**](https://github.com/NVIDIA/nccl) - Optimized primitives for collective multi-GPU communication across PCIe and InfiniBand.
* [**Jails for NetBSD**](https://netbsd-jails.petermann-digital.de/) - Bringing kernel-enforced isolation and container-like resource control to NetBSD.
* [**FnNAS for Arm64 Devices**](https://github.com/ophub/fnnas) - A deeply customized Debian-based OS for Arm64 TV boxes acting as NAS servers.
* [**NVIDIA Driver Installation on openSUSE/SLE**](https://sndirsch.github.io/nvidia/2025/07/16/nvidia-drivers.html) - A definitive guide to GFX, CUDA, and open-kernel drivers on SUSE.

## AI, Agents & Tools

* [**Nano Banana 2: Google's Latest AI Image Model**](https://blog.google/innovation-and-ai/technology/ai/nano-banana-2/) - Google combines the power of Nano Banana Pro with Gemini Flash for rapid AI editing.
* [**Firefox 148 AI Kill Switch**](https://serverhost.com/blog/firefox-148-launches-with-exciting-ai-kill-switch-feature-and-more-enhancements/) - Firefox gives users explicit control to disable AI-generated summaries and chatbot prompts.
* [**Evaluating AGENTS.md for Coding Agents**](https://arxiv.org/abs/2602.11988) - Research suggesting that over-specifying context for AI agents can actually decrease success rates.
* [**Choosing an Inference Engine: Why Choice Matters**](https://www.suse.com/c/choosing-an-inference-engine-why-choice-matters/) - A comparison of vLLM, TGI, and llama.cpp for production environments.
* [**AI World Clocks**](https://clocks.brianmoore.com/) - A creative experiment generating unique analog clocks every minute using LLMs.

## Linux, Systems & Hardware

* [**Building a Low Power Server (Part II)**](https://osint.quest/blog/building-a-low-power-server-part-2/) - Optimizing BIOS C-States and ASPM to achieve a 14.5W idle power draw.
* [**Floppy Disks to Run SF Trains Until 2030**](https://arstechnica.com/gadgets/2024/04/5-25-inch-floppy-disks-expected-to-help-run-san-francisco-trains-until-2030/) - A fascinating look at the longevity of legacy hardware in critical infrastructure.
* [**Even the Mars Rover Uses Zip Ties**](https://www.thedrive.com/tech/39426/even-the-mars-rover-has-zip-ties) - Highlighting the reliability of Tefzel zip ties in extreme extra-planetary environments.
* [**Nearby Glasses Detection App**](https://github.com/yjeanrenaud/yj_nearbyglasses) - An Android tool attempting to detect smart glasses using Bluetooth Low Energy.
* [**Apple's "Breathing Light" Sleep Indicator**](https://unsung.aresluna.org/just-a-little-detail-that-wouldnt-sell-anything/) - A nostalgic look at one of Apple's most human-centric design details.
* [**12" MacBook Retina Logic Board Failure**](https://discussions.apple.com/thread/8520071?sortBy=rank) - Community analysis of the U4700 controller issues plaguing the ultra-thin MacBook.
* [**Diode: Hardware Simulation in the Browser**](https://www.withdiode.com/) - Build and simulate hardware circuits with a clean, web-native schematic interface.

## Development, Web & Tools

* [**Charm v2 Terminal Tooling**](https://charm.land/blog/v2/) - Major updates to Bubble Tea and Lip Gloss optimized for the era of AI coding agents.
* [**dotenvx**](https://dotenvx.com/) - A secure, encrypted version of dotenv from its original creator.
* [**enject (formerly enveil)**](https://github.com/GreatScott/enveil) - Protecting your `.env` secrets from leaking into AI coding tool prompts.
* [**Authentik**](https://github.com/goauthentik/authentik) - The open-source identity provider that's becoming a go-to for self-hosted SSO.
* [**Kanidm**](https://kanidm.com/) - A modern identity management platform written in Rust with native Webauthn support.
* [**Conventional Responses**](https://conventionalresponses.org/) / [**Comments**](https://conventionalcomments.org/) / [**Commits**](https://www.conventionalcommits.org/en/v1.0.0/) - Standards for improving human and machine-readable communication in development.
* [**Omarchy-Inspired macOS Setup**](https://www.penkin.me/development/tools/productivity/configuration/2025/11/28/building-omarchy-inspired-setup-macos.html) - Building a keyboard-driven, tiled workflow on macOS using yabai and skhd.
* [**Homio Home Assistant Dashboard**](https://github.com/iamtherufus/Homio) - A clean, YAML-based dashboard optimized for tablets and mobile devices.
* [**Wallabag + Kobo Offline Reading**](https://bnolet.me/posts/2024/11/wallabag-kobo-offline-reading-bliss/) - Creating a distraction-free "read it later" workflow using KOReader.
* [**Hacking an old Kindle to display bus arrival times**](https://www.mariannefeng.com/portfolio/kindle/) - A creative project detailing how to jailbreak and repurpose an old Kindle as a low-power E-Ink dashboard for real-time bus tracking.
* [**Libertinus Font Family**](https://github.com/alerque/libertinus) - A robust open-source font family with excellent math support.

## Gaming, Fun & Misc

* [**Gran Turismo 4 Spec II Mod**](https://www.theadmiester.co.uk/specii/) - Spec II is a mod which expands upon the core Gran Turismo 4 experience, bringing a variety of fixes and improvements to the game.
