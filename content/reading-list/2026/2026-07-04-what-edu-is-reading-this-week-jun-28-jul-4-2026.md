---
title: "What Edu is reading this week (Jun 28 - Jul 4, 2026)"
date: 2026-07-04T07:00:00+02:00
draft: false
slug: 2026-07-04-what-edu-is-reading-this-week-jun-28-jul-4-2026
aliases:
  - /posts/2026-07-04-what-edu-is-reading-this-week-jun-28-jul-4-2026/
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
  - sdr
---

A week centred on running LLMs locally, new model releases from Anthropic and the government vetting of others, a big Immich release and self-hosting tooling, a couple of unsettling disk-encryption and firmware stories, and reviving old hardware.

![What Edu is reading this week (Jun 28 - Jul 4, 2026)](/images/2026-07-04-what-edu-is-reading-this-week-jun-28-jul-4.png)

## AI, Models & Coding

* [**local-inference-lab/rtx6kpro**](https://github.com/local-inference-lab/rtx6kpro) / [**jamesob/local-llm**](https://github.com/jamesob/local-llm): A wiki on running large LLMs (Qwen3.5-397B, Kimi-K2.5, GLM-5) on PCIe GPUs without NVLink, plus a companion "everything I know about running LLMs locally" collection.
* [**Qwen 3.6 27B is the sweet spot for local development**](https://quesma.com/blog/qwen-36-is-awesome/): Why Qwen 3.6 27B is finally a model good enough for coding locally on a MacBook or an RTX, using llama.cpp and OpenCode.
* [**Self-Host GLM 5.2: Open Weights & vLLM Guide**](https://lushbinary.com/blog/glm-5-2-self-hosting-open-weights-vllm-guide/): A planning guide for self-hosting GLM 5.2 — VRAM budget formula, ~744 GB FP8 weights, KV cache for 1M context, and vLLM vs SGLang.
* [**llm-d — SOTA LLM inference on any accelerator**](https://llm-d.ai/docs/getting-started): An open-source inference serving stack for Kubernetes that runs vLLM, SGLang and more across a cluster on NVIDIA, AMD and custom accelerators.
* [**Introducing Claude Sonnet 5**](https://www.anthropic.com/news/claude-sonnet-5) / [**Redeploying Claude Fable 5**](https://www.anthropic.com/news/redeploying-fable-5): Anthropic's most agentic Sonnet yet, and the redeployment of Fable 5 from July 1 after export controls were lifted, with updated cybersecurity safeguards.
* [**Senior SWE-Bench**](https://senior-swe-bench.snorkel.ai/): A benchmark from Snorkel that evaluates agents as senior engineers on the kind of work actually handed to them.
* [**headroomlabs-ai/headroom**](https://github.com/headroomlabs-ai/headroom): Compress tool outputs, logs, files and RAG chunks before they reach the LLM — 60-95% fewer tokens for the same answers, as a library, proxy or MCP server.
* [**OpenClaw is now on iOS + Android**](https://x.com/openclaw/status/2071688039114342592): Native mobile apps for OpenClaw, with channels, tasks and replies so you can run agents from your phone.
* [**Built-in Co-Authored-By: Claude commit trailer**](https://github.com/anthropics/claude-code/issues/66602): An issue arguing that Claude Code's default commit trailer asserts AI co-authorship, contrary to U.S. Copyright Office guidance.
* [**U.S. government will decide who gets to use the latest ChatGPT upgrade**](https://www.washingtonpost.com/technology/2026/06/26/openai-says-us-government-will-vet-users-its-latest-ai-model/): OpenAI says the government will vet users of its newest model, as the administration increases oversight of the industry.

## Cloud, Containers & Kubernetes

* [**ngrok/webernetes**](https://github.com/ngrok/webernetes) / [**I ported Kubernetes to the browser**](https://ngrok.com/blog/i-ported-kubernetes-to-the-browser?ref=selfh.st): Kubernetes running in the browser — almost 100,000 lines of LLM-generated code in two months, with the story of how it was built.
* [**Podman 6 Configuration File Changes**](https://blog.podman.io/2026/06/podman-6-configuration-file-changes/): Ahead of the Podman 6 release, a rundown of the biggest change: a major rework of how configuration files are handled and parsed.
* [**Red Hat Enterprise Linux runner images in public preview**](https://github.blog/changelog/2026-06-25-red-hat-enterprise-linux-runner-images-are-now-in-public-preview/): GitHub-hosted larger runners now support RHEL 9 and RHEL 10 images, in partnership with Red Hat.

## Self-Hosting & Homelab

* [**Immich v3.0.0**](https://github.com/immich-app/immich/discussions/29439): The next major version of Immich after months of work, with breaking changes worth reading before you upgrade.
* [**romainrbr/immich-face-to-album**](https://github.com/romainrbr/immich-face-to-album) / [**TrooP81/Immich-ppl2album**](https://github.com/TrooP81/Immich-ppl2album/): Two small tools to sync Immich faces into specific albums automatically.
* [**PixelUnion — Free your photos from American tech platforms**](https://pixelunion.eu/es/) / [**Immich FAQ**](https://pixelunion.eu/help/immich/immich-faq/): A managed Immich hosting service pitched on privacy, plus its FAQ on Immich features and compatibility.
* [**I Don't Maintain My Homelab**](https://cleberg.net/blog/homelab-maintenance.html?ref=selfh.st): An argument for a homelab that maintains itself rather than demanding constant attention.
* [**Jcorp Nomad: a self-hosted media server that fits in your pocket**](https://old.reddit.com/r/selfhosted/comments/1ugjh28/jcorp_nomad_a_self_hosted_media_server_that_fits/): A pocket-sized self-hosted media server project, well received on r/selfhosted.
* [**jomjol/AI-on-the-edge-device**](https://github.com/jomjol/AI-on-the-edge-device): An easy-to-use device for connecting "old" analog meters (water, power, gas) to the digital world.

## Linux & Systems

* [**FreeBSD ate my ram!**](https://crocidb.com/post/freebsd-ate-my-ram/): A month spent researching FreeBSD's virtual memory system to understand why htop, btop and fastfetch disagree about RAM usage — ending in patches to all three.
* [**NUMA Explained: Why Memory Distance Slows Your VMs**](https://edera.dev/stories/numa-part-1-cores-memory-and-the-distance-between-them): Why two identical VMs on the same host can perform 20% differently, and what NUMA topology actually costs you.
* [**Linux on Older Hardware: The Complete Revival Guide (2026)**](https://www.fosslinux.com/158206/linux-on-older-hardware-revival-guide.htm): Lightweight distros, zram tuning, SSD upgrades and browser tweaks tested on a 2014 ThinkPad.
* [**Researchers turn old Pixel phones into a data center**](https://www.techspot.com/news/112762-researchers-turning-old-pixel-phones-data-center-they.html): Google Research reuses old Pixels — framed around "embodied carbon" — into a cluster that outperforms some server hardware.

## Security

* [**A LUKS encryption key that lingered in RAM across suspend**](https://mathstodon.xyz/@iblech/116769502749142438): A git-bisecting saga: since Linux 6.9 the tool locking a laptop's LUKS drive on suspend was silently failing, leaving the key in memory — fixed with a single line.
* [**Claude Code Is Steganographically Marking Requests**](https://thereallo.dev/blog/claude-code-prompt-steganography): An inspection of Claude Code that found hidden system-prompt markers derived from the API base URL and timezone.
* [**PS5 Linux loader 2.2**](https://x.com/theflow0/status/2071885242562912407): Andy Nguyen ("TheFlow") announces version 2.2 of the PS5 Linux loader, adding support for PS5 firmware 7.61.

## SDR, Hardware, Gaming & Misc

* [**Internal Combustion Engine — Bartosz Ciechanowski**](https://ciechanow.ski/internal-combustion-engine/): Another of Ciechanowski's beautiful interactive explainers, this time on how an internal combustion engine actually works.
* [**The BBC's Long Wave signs off after 101 years**](https://x.com/RadioHacking/status/2070664763286110209): The BBC's Long Wave broadcast went silent at 00:00 UTC — its last minute captured after the Shipping Forecast, with the notes of God Save the King and an automated end-of-transmission notice.
* [**Physical disc production ending in January 2028 for new PlayStation games**](https://blog.playstation.com/2026/07/01/physical-disc-production-ending-in-january-2028-for-new-games-releasing-on-playstation-consoles/): New PlayStation games will ship in digital-only formats, reflecting shifting consumer preferences.
* [**OpenRA**](https://www.openra.net/): Classic real-time strategy games (Command & Conquer, Red Alert, Dune 2000) rebuilt for the modern era.
* [**Ferrari's marketing boss quits weeks after EV launch backlash**](https://www.bbc.com/news/articles/cnv9edrjjn4o): The design of Ferrari's first all-electric car, the Luce, was heavily criticised.
* [**rajtilakjee/kivo**](https://github.com/rajtilakjee/kivo): A lightweight desktop teleprompter.
* [**HCCF's vision for a human-centered top-level domain**](https://hccf.onmy.cloud/2026/06/21/reclaiming-our-digital-selves-hccfs-vision-for-a-human-centered-top-level-domain/): The Human-Centered Computing Foundation makes the case for reclaiming our digital selves through a new human-centered TLD.