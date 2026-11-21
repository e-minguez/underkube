---
title: "What Edu is reading this week (Nov 15 - 21, 2026)"
date: 2026-11-21T07:00:00+01:00
draft: false
slug: 2026-11-21-what-edu-is-reading-this-week-nov-15-21-2026
aliases:
  - /posts/2026-11-21-what-edu-is-reading-this-week-nov-15-21-2026/
categories:
  - Reading
tags:
  - newsletter
  - links
  - tech
  - security
  - linux
  - ai
  - networking
  - homelab
  - hardware
  - sdr
  - gaming
  - testing
---

Two unauthenticated remote code execution bugs in nginx lead the security reading this week, next to a KVM guest-to-host escape that sat in the kernel for four years and Jensen Huang leaving Nvidia after 33 years. Around them, Gemini 4 Neon and Qwen4-Max landing two days apart, GTA 6 reviews after a hundred hours in Vice City, and a strong week for property-based testing.

## Security

* [**Unauthenticated remote code execution in NGINX**](https://www.wiz.io/blog/nginx-http2-rce-vulnerabilities) / [**NGINX2Root**](https://xint.io/blog/nginx2root-remote-code-execution) - CVE-2026-123633 and CVE-2026-123007, found independently by Wiz Research, Ikotas Labs, Metnir, Rapid7 and Xint, are critical pre-authentication RCEs in nginx that need HTTP/2 enabled. The integer underflow dates back to 1.9.5 in 2015 and the use-after-free is nearly six years old; Xint counts five CVEs in the set (HTTP/3 and the mail proxy included), chains one with an SCTP kernel bug to get root on the host and escape a Docker container, and notes that turning HTTP/2 off only blocks two of the five. Fix is 1.31.9, and Wiz credits AI harnesses for finding what a decade of humans missed.
* [**OpenSSL: buffer overflow in EVP_EncodeBlock()**](https://news.ycombinator.com/item?id=50569226) - The thread on CVE-2026-121481, CVSS 9.8, with most of the 329 comments about the function itself: EVP_EncodeBlock encodes base64, it malfunctions when the caller feeds it more than roughly 1.5 GB, and the API never takes an output buffer length, so the implementation has nothing to check against.
* [**tldrcve: CVEs in plain English**](https://tldrcve.com/) - Answering the two questions most of us actually have about a CVE: are you affected, and what should you do. Every entry gets a scare-o-meter rating (the OpenSSL base64 bug is a shrug, since it needs 1.5 GB of input you supply and no remote path is known) and the November PHP and Ruby rounds are listed with the configuration each one really needs.
* [**KVM guest-to-host escape**](https://www.terra.security/blog/kvm-guest-to-host-escape) - CVE-2026-99312: on AMD hosts with nested virtualization enabled, a guest can read memory that belongs to the physical host, demonstrated on a DigitalOcean droplet. The flaw sat in KVM for just under four years and was opened by an earlier security fix, and the write-up walks through the nested page table that is meant to prevent exactly this.
* [**Universal XSS in uBlock Origin**](https://iter.ca/post/ubo-uxss/) - A one-click UXSS in the MV2 Firefox build of uBO, with the MV3 Lite build affected less severely: a malicious site drove the element picker into adding an arbitrary trusted filter, and trusted filters can inject JavaScript, so the attacker could run code in the context of any site. GPT-5.6 Sol did most of the discovery work. Fixed.

## AI, Models and Agents

* [**Introducing Gemini 4 Neon**](https://blog.google/innovation-and-ai/models-and-research/gemini-models/introducing-gemini-4-neon/) - $3 per million input tokens and $15 per million output, cached input at $0.15, a million-token context. Google puts Neon third overall on the Artificial Analysis Intelligence Index at 61 at its xhigh thinking level, second on the Vals Index and second on steerability in the new Agent Arena Index, and reports its lowest fabrication rate yet in internal Antigravity testing.
* [**Qwen4-Max**](https://qwen.ai/blog?id=qwen4-max) - Alibaba's new flagship runs on the Qwen4 architecture with a 2.4-trillion-parameter backbone, native vision and a one-million-token context window, framed as a teammate for work, creativity and discovery.
* [**The components of agent memory**](https://www.anthropic.com/research/components-of-agent-memory) - An agent has to decide what is worth remembering before it knows what happens next, which is the same bind Kierkegaard described. The piece walks through how a "dreaming" pass consolidates experience offline the way sleep consolidates memory in the hippocampus, while the moment-to-moment encoding stays cheap.
* [**Introducing ambient agents**](https://www.langchain.com/blog/introducing-ambient-agents) - Agents that are not started by a chat message: they listen to an event stream and act on many events at once. The post lays out the three human-in-the-loop patterns (notify, question, review) and builds them into an open source email assistant with LangGraph.
* [**the answer to ai is engineering**](https://ghuntley.com/answer/) - Huntley's AI DevCon New York talk: security take-off is the new normal, you do not need most open source libraries any more, and a Nix overlay lets you patch the whole world, with a closing round on loops, back pressure and property-based testing.

## Linux and Systems

* [**clifr**](https://github.com/jlruedab/clifr) - A flight recorder for Linux servers. clifrd runs as a service and keeps 72 hours of state in /var/lib/clifr, including processes that lived milliseconds, plus connections, open files and counters, using eBPF at about 2% of one CPU core on a busy server. The query tool then rebuilds the output of ps, top, ss, lsof, df, vmstat, dmesg and about 40 commands as they would have looked at any past moment. AGPL-3.0.
* [**Sashiko**](https://sashiko.dev/) / [**sashiko-dev/sashiko**](https://github.com/sashiko-dev/sashiko) - An agentic code review system for the Linux kernel, with profiles for GCC, QEMU, Zephyr RTOS and itself: project-specific prompts, source-verified code notes and a multi-stage verification protocol, reviewing patches locally from a git checkout or automatically from mailing lists and forges. The front end shows live kernel patch reviews and tracked bugs.
* [**Disk encryption on NetBSD**](https://www.reddit.com/r/NetBSD/s/tZ8zsBMbfh) - The r/NetBSD link to Nia Alarie's write-up on what disk encryption can and cannot give you. Start from the threat model (a stolen device first, tampering later) and from the fact that base system binaries are the ones everyone else runs, and the set of directories that matter shrinks to /home, /var and /root, with /rescue for when shared libraries are gone and Adiantum for CPUs without AES.
* [**9/UX: a Macintosh-inspired desktop for 9front**](https://progrium.github.io/9ux/) - The classic Mac and A/UX desktop (spatial desktop, global menu bar, consistent controls and dialogs) rebuilt for Plan 9's 9front. It runs live in the browser through h9 and its own 386 emulator, about 23 MB once, with the demo being the real thing rather than a video.
* [**The secret ThinkPad powerbutton code**](https://masnick.com/posts/the-secret-thinkpad-powerbutton-code-to-bring-dead-laptops-back-to-life/) / [**HN discussion**](https://news.ycombinator.com/item?id=50516473) - The 2007 post about the key sequence that brings a dead ThinkPad back, and a thread where a former call centre operator offers the likely real explanation: asking for ten one-second presses is a reliable way to make sure the customer actually holds the button long enough.

## Storage, Networking and Homelab

* [**croit ceph-rust**](https://github.com/croit/ceph-rust) - Ceph rewritten from scratch in Rust and wire-compatible with v21.2.0 and v20.2.4 clusters: FlashStore as an OSD built for NVMe (thread per core, lock-free hot paths, acknowledged only once durable), librustyrados, librustyrbd and librustycephfs, io_uring TCP by default with optional RoCEv2 and GPUDirect RDMA through a NIXL plugin. It drops into an existing cluster one drive or one server at a time, and the OSD tunes its own cores, queues and memory.
* [**Who's delivering GTA 6?**](https://labs.ripe.net/author/emileaben/whos-delivering-gta-6-a-ripe-atlas-measurement-story/) - How do you deliver a 200 GB game to millions of players? RIPE Atlas measurements taken during the pre-load, looking at what DNS and the content delivery networks behind PlayStation and Xbox do under that load.
* [**ph-intercept**](https://ph-intercept.com/) - Every DNS query on your network becomes a ship: allowed ones cruise past, blocked ads, trackers and malware get shot down, and you can flip blocking or update your lists from the HUD. Works with Pi-hole, AdGuard Home and Technitium, one container to run, and it is on Unraid Community Apps.
* [**A $2-3/mo VPS is the best remote access solution**](https://www.reddit.com/r/selfhosted/comments/1xy63oj/a_23mo_vps_is_the_best_remote_access_solution/) - The r/selfhosted case for a two or three dollar VPS over the Cloudflare and Tailscale route into your own network: those are fine, in the poster's view, but they spoil the point of self hosting.
* [**What is w2rt6byl5nf1opmc-a.com?**](https://jack.cab/blog/siterate) - A backlink monitor fires, the new backlink is spam, and the trail leads to a site that ranks the web by linking subnets: the random domain sits at number 8 in the .com list and number 8 in the Majestic Million, two days after registration, with 241 million nofollow backlinks and no working DNS. A good look at the spam backlink economy and the people who rank by it.

## Development and Testing

* [**In praise of property-based testing**](https://increment.com/testing/in-praise-of-property-based-testing/) / [**Hypothesis**](https://hypothesis.works/) / [**Hegel**](https://hegel.dev/) - David MacIver's article makes the case for testing properties instead of examples, Hypothesis is the Python library he built for it (it picks the inputs and shrinks a failure to the simplest example that still fails), and Hegel is the universal property-based testing engine and multi-language library family built on Hypothesis, partly by Hypothesis developers at Antithesis.
* [**Property-based testing, how it works and when to use it**](https://antithesis.com/docs/resources/property_based_testing/) / [**Bombadil**](https://github.com/antithesishq/bombadil) - Antithesis on where property-based testing sits next to fuzzing and generative testing and which systems benefit, plus Bombadil, its Rust tester for web and terminal UIs that explores an application and validates the correctness properties you declare, locally, in CI or inside Antithesis.
* [**Why notification systems are a nightmare for engineers**](https://notifkit.dev/articles/why-notification-systems-are-a-nightmare) - Sending one email is one line of code, and sending them properly is something else. The article follows that line of code as it grows, one support ticket at a time, through seven incidents at real companies.

## Hardware, Radio and Making

* [**Flipper One**](https://www.kickstarter.com/projects/flipper-devices/flipper-one/) - Flipper Devices' open Linux multi-tool, built on a powerful ARM processor and pitched as a network toolkit that expands with modules. The device is on Kickstarter.
* [**ChameLab**](https://m0n5ter.github.io/ChameLab/) - Desktop, mobile and web app for the ChameleonUltra and ChameleonLite, with an extended firmware and a command line client. All eight slots at a glance with drag to reorder, HF and LF edited separately, and an LF slot that can hold up to eight cards of different emulated types. GPL v3, one app for Windows, macOS, Linux, Android and the browser.
* [**UV5R mini community firmware 1.1.0**](https://www.reddit.com/r/Baofeng/comments/1xzby6w/uv5r_mini_community_firmware_110_released/) / [**MM9PDY firmware docs**](https://github.com/pskillen/mm9pdy-firmware/blob/main/docs/baofeng-uv5rmini/README.md) - The humble UV-5R Mini gets zones, single watch and a programmable front key, while the MM9PDY project ships the manufacturer's firmware with tested features added for the UV-5R Mini, the DM-32UV, the AT-D890UV and a couple of Retevis boards, installed from the browser and checked against your stock version before anything is written.
* [**ESP32 Flash Encryption Explained**](https://www.youtube.com/watch?v=GyAqlYea8wU) / [**guide and scripts**](https://github.com/UsableLoki8221/GUIDE---ESP32_Flash_Encryption) - A video walkthrough of flash encryption and burning the eFuses by hand, plus the repo that automates it: generate and store a key, burn the fuses to the state you want, then flash encrypted or plaintext by detecting the crypt fuse on the board. The note at the end is that OTA updates are still plaintext unless you secure them separately.
* [**Logitech Harmony IR archive**](https://github.com/pickysysadmin/logitech-harmony-ir-archive) - The infrared control database from Logitech's Harmony remotes, rescued before it disappeared with the service: about 276,000 devices from 7,900 manufacturers, 13.3 million commands and all 684 of Logitech's own IR protocol definitions, as plain JSON with original keycodes and ready-to-send Pronto Hex. CC0.

## Desk Companions and Displays

* [**ClawPal**](https://github.com/Kaayoos/clawpal) - A Waveshare ESP32-S3 touch display turned into a desk companion: a pixel crab showing CPU and GPU load and temperatures, a 60-second network chart, media controls with a per-app volume mixer, your Claude Code and Codex limits with reset countdowns and a pace forecast, weather, clock and timer. GPL-3.0, C.
* [**deskbuddy**](https://github.com/Shriaman2005/deskbuddy) - The cheap version of the same idea: any Android phone, with Chip as a pixel-art face inside Termux that blinks, reacts to touch, wears headphones when music plays, types along while you work and turns your voice into typing on the laptop. Home Wi-Fi only, no cloud, no account, no camera, and it was built on a Galaxy M01 Core.
* [**The MacBook Pro's OLED PWM problem**](https://macanorak.com/the-macbook-pros-oled-pwm-problem-when-a-better-display-becomes-worse-to-use/) - Apple made a spectacular display, and the argument is that spectacular is not the same as comfortable: a look at pulse-width modulation on the OLED MacBook Pro and at the people who notice it, with the request that they be heard.

## Gaming, Fun and Misc

* [**GTA 6 review**](https://www.ign.com/articles/grand-theft-auto-vi-review) - IGN after more than a hundred hours in and around Vice City, nearly 120 to the credits: Jason and Lucia are after escape rather than revenge or empire building, and the verdict is that nothing has hit quite like it.
* [**NMS Optimizer**](https://nms-optimizer.app/?platform=standard) - A free, open source, ad-free calculator for No Man's Sky tech layouts: pick your platform, choose the tech, mark the supercharged slots, and it searches the grid (up to roughly 10^81 possible layouts) for adjacency bonuses, typically 15 to 20% better than arranging by hand.
* [**Auto Modellista recomp**](https://github.com/apexJCL/automodellista-recomp) - The Xbox racing game turned into a native game for Windows, macOS and the Steam Deck with no emulator: a builder wizard takes your own disc image, checks its fingerprint against the single supported release, and builds an install.
* [**Nintendo takes Picofly firmware off GitHub**](https://www.youtube.com/watch?v=-TLCGUpoD6c) - A video whose description points to the Consumer Rights Wiki write-up: a DMCA notice from Nintendo of America dated 6 November disabled 144 repositories, the firmware for Picofly among them, a chip soldered into the Switch. The notice leans on the anti-circumvention clause and the Team Xecuter case; consoles already fitted keep working, but owners lose the simple way to update them.
* [**Watched**](https://www.watched.earth/) - Enter any place on Earth and see every satellite that passed over it in the last seven days, with the pictures they took. The orbit maths for about 400 imaging, weather, radar and crewed satellites runs in your browser, and it matches passes against Sentinel-2, Landsat, Sentinel-1 and weather imagery, checking whether your spot was under cloud.
* [**Ovoko**](https://ovoko.es/) - A Spanish marketplace for used car parts and accessories with a return guarantee, and a catalogue that covers all car models.

## Learning and Making

* [**CS Learn**](https://www.cs.cmu.edu/learn/) / [**HN discussion**](https://news.ycombinator.com/item?id=50522980) - Carnegie Mellon released full semesters of lectures from current computer science courses on YouTube, free, one course premiering each day during launch week and more in January. Phillip Compeau answers the thread himself, and the part worth reading is how the courses got out: students built tools that automate much of the production work, so a small team can ship one.
* [**How to make (almost) anything**](https://pub.cba.mit.edu/863.26/site/) / [**HN discussion**](https://news.ycombinator.com/item?id=50514470) - MIT's MAS.863 course site with the 2026 schedule, from computer-aided design and computer-controlled cutting through embedded programming, electronics design and production, output devices and edge AI. The thread argues breadth against depth, and the case for breadth is that knowing something exists is what turns a dead end into a search.
* [**Basic Beginners FreeCAD v1**](https://www.youtube.com/playlist?list=PLWuyJLVUNtc3UYXXfSglVpfWdX31F-e5S) - A new video course for FreeCAD v1 aimed at beginners, built around translating real world objects into the digital realm, which is the CAD thinking more than the buttons.

## Industry and Work

* [**Microsoft CEO explains why he asked 60K employees to quit**](https://techcrunch.com/2026/11/18/microsoft-ceo-satya-nadella-explains-why-he-asked-60k-employees-to-quit/) - The October buyouts were the AI-first transformation with a door attached. Nadella's argument is that a 51-year-old incumbent has to change the work, the workflow and the work artifact, that this takes longer than anyone expects, and that people should get to choose whether to come along. He also concedes the industry created enormous anxiety by talking about the singularity.
* [**What's next for Nvidia?**](https://steveblank.com/2026/11/15/whats-next-for-nvidia/) - Nvidia's board announced that Jensen Huang resigned 33 years after he co-founded the company, and Steve Blank asks the question that usually ends badly: what happens when the visionary leaves. He counts three reinventions, CUDA in 2006 funded years ahead of revenue, deep learning after ImageNet in 2012, and Mellanox in 2020 turning boards into AI datacenter racks.
* [**Amazon's decoy deals**](https://groundworkcollaborative.org/news/amazons-decoy-deals-groundwork-investigation-reveals-nearly-1-in-3-black-friday-and-cyber-monday-deals-advertised-by-amazon-offered-no-savings-to-shoppers-nearly-1-in-10-w/) - A Groundwork Collaborative investigation of Black Friday and Cyber Monday listings finds nearly one in three of the deals Amazon advertised offered no savings, and nearly one in ten were actually more expensive than they had been.
* [**OccupySaaS**](https://occupysaas.com/) - Laid-off engineers building clean room, AI-assisted, open source, drop-in replacements for the SaaS platforms they used to work on: Apache-2.0, self-hosted, no per-seat tax. The first release is ZeroAuthy v1.0.0-rc.1, and the site is upfront that this is a protest movement written in code.

