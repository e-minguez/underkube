---
title: "What Edu is reading this week (Oct 4 - 10, 2026)"
date: 2026-10-10T09:00:00+02:00
draft: false
slug: 2026-10-10-what-edu-is-reading-this-week-oct-4-10-2026
aliases:
  - /posts/2026-10-10-what-edu-is-reading-this-week-oct-4-10-2026/
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
  - gaming
  - sdr
---

This week's list is heavy on decompilations and native ports of old console games, next to a good batch of agentic tooling and a few infrastructure moves worth noting (gVisor into the CNCF, Deno into Cloudflare).

## Cloud, Infrastructure & Open Source

* [**gVisor is being donated to CNCF**](https://gvisor.dev/blog/2026/10/02/gvisor-cncf/) - The application kernel sandbox moves under the CNCF umbrella.
* [**Deno is joining Cloudflare**](https://deno.com/blog/cloudflare) - The runtime team explains why joining Cloudflare is the best place to keep building for the web.
* [**Our $445M Series D**](https://oxide.computer/blog/our-445m-series-d) - Oxide Computer raising another round for its rack scale on prem cloud.
* [**containers/fetchit**](https://github.com/containers/fetchit) - Manages the life cycle and configuration of Podman containers straight from Git.
* [**The people holding up the internet**](https://sheets.works/data-viz/holding-up-the-internet) - Data drop that counts who actually maintains 23 pieces of software that phones, browsers and servers depend on, and finds 11 of them resting on one or two people. Paul Eggert keeps the time zone database in his spare time, Todd Miller made 5,408 of the 5,409 sudo changes between 2008 and 2018, and Lasse Collin's xz story is in there too.

## AI, Agents & Tools

* [**Hermes Index | Agentic Model Leaderboard**](https://portal.nousresearch.com/bench#leaderboard) - Task completion and cost per task across Hermes Bench, TerminalBench 4, TerminalBench Science and SkillsBench.
* [**morluto/rea**](https://github.com/morluto/rea) - Reverse engineering with agents, from app behaviour down to native binaries.
* [**franzenzenhofer/big-arrow-on-the-screen**](https://github.com/franzenzenhofer/big-arrow-on-the-screen) - A CLI skill that lets AI agents paint arrows, boxes and text on your Mac screen, click through and self erasing.
* [**ArtCraft**](https://getartcraft.com/) - Open desktop app for generating AI video and images.
* [**Whistle: Speech to Text in 16.9 MB**](https://cactuscompute.com/blog/whistle) / [**Hacker News discussion**](https://news.ycombinator.com/item?id=50008427) - An open speech recognition model on the same CPU engine as Needle: seven languages, first token in 11 ms.
* [**Decisions API is in public beta**](https://developers.openai.com/api/docs/guides/decisions) / [**Hacker News discussion**](https://news.ycombinator.com/item?id=49984025) - Check conditions, select from fixed options and score text and images against a rubric.
* [**Introducing Playground: Create and play custom games**](https://blog.google/innovation-and-ai/technology/ai/playground-experimental-gaming-platform/) / [**playground.google**](https://playground.google/explore) - Google's experimental platform for creating, playing and sharing custom games with AI.
* [**The end of software secrecy is almost upon us**](https://x.com/esrtweet/status/2106983467141509385) - Eric S. Raymond on decompilation closing the gap between closed and open source.

## Linux, Systems & Hardware

* [**M-Abozaid/esp32-c3-adblock**](https://github.com/M-Abozaid/esp32-c3-adblock) - Pi hole class DNS ad blocker on a $2 ESP32-C3: 537k domains as 40 bit FNV-1a hashes in flash, binary searched, plus a web dashboard.
* [**adswill/OnAir**](https://github.com/adswill/OnAir) - Free SDR receiver app for macOS, Windows and Linux: digital TV (DVB-T/T2, ATSC) and DAB radio with a HackRF and friends.
* [**vmm(4)/vmd(8) gain support for multi-processor VMs**](https://undeadly.org/cgi?action=article;sid=20260927115632) - OpenBSD's hypervisor now handles multi processor guests.
* [**Huge news for the NetBSD community**](https://www.reddit.com/r/NetBSD/comments/1wzpvlm/huge_news_for_the_netbsd_community_today/) - The yearly funding campaign closed with $120,282 raised against a $50,000 goal.

## Retro Gaming, Native Ports & Recompilations

* [**PC ports of old console games are the new AI vibe coding battleground**](https://www.pcgamer.com/gaming-industry/pc-ports-of-old-console-games-are-the-new-ai-vibe-coding-battleground/) - PC Gamer on the wave of decompilation and recompilation projects.
* [**carafe-nx/carafe**](https://github.com/carafe-nx/carafe) - Desktop app that turns Windows games into Switch apps.
* [**Start a new decomp project**](https://github.com/Druthulu/BFM-decomp/wiki/Start-a-new-decomp-project) - Wiki from the Brave Fencer Musashi matching decompilation, where 218 binaries rebuild byte identical from C.
* [**BenMcLean/CloudyQuake**](https://github.com/BenMcLean/CloudyQuake) - Multiplayer Quake playable straight in the browser, pointed at your own dedicated server.
* [**Nyaldee/Ports-Launcher**](https://github.com/Nyaldee/Ports-Launcher) - Rust library manager and installer for unofficial native game ports and recomps, portable and with zero runtime dependencies on Windows, Linux and Android.
* [**SpeedBreakerProject/speedbreaker**](https://github.com/SpeedBreakerProject/speedbreaker) - Static recompilation of the Xbox 360 version of Need for Speed: Most Wanted (2005), with native builds for Steam Deck, Linux and Mac.
* [**Odrannnn/MetroidPrimePort**](https://github.com/Odrannnn/MetroidPrimePort) - Native port of Metroid Prime for Linux, Windows and Android built from the PrimeDecomp decompilation, bring your own disc image.
* [**LoreanXavier/pt-pc**](https://github.com/LoreanXavier/pt-pc) - Native PC port of P.T. that runs from your own PS4 game files.
* [**deadinside28/bloodborne_pc**](https://github.com/deadinside28/bloodborne_pc) - C++ project working towards Bloodborne on PC, with a few thousand stars behind it.
* [**Golden Sun has a PC and Android recomp now**](https://www.reddit.com/r/decomps/comments/1wzgi3i/golden_sun_has_a_pc_and_android_recomp_now/) - r/decomps thread on the new native builds.
* [**Tiny Hell (Playdate)**](https://campalans.itch.io/tiny-hell-playdate) - Find the enemy you cannot see: crank, aim, fire, survive.
* [**ArduDate**](https://bitcalibergames.itch.io/ardudate) - An Arduboy emulator for the Playdate.
* [**PLAY-DOS**](https://playdos.albertomartinfernandez.com/) - Browser tribute to MS-DOS with 5,921 curated games from softwarelibrary_msdos_games, plus quizzes and a small synth behind a CRT screen.
* [**My Internet Archive browser is now available for Steam Deck**](https://www.reddit.com/r/SteamDeck/comments/1wz41zs/my_internet_archive_browser_is_now_available_for/) - The Archivist Browser ported to the Deck.

## Development & The Web

* [**We ported the original Doom to SQL**](https://cedardb.com/blog/sqldoom/) - CedarDB running Doom inside a database, one query at a time.
* [**Beauty in DVD Menus**](https://vale.rocks/posts/dvd-menus) - A look at the craft of DVD menu design and why it still holds up.
* [**Example.com Just Launched The Biggest Redesign In Decades**](https://www.debugbear.com/blog/example-dot-com-redesign-history) - DebugBear walks through the visual history of example.com.
* [**BIGWORDS.PAGE**](https://bigwords.page/) - Turns a phone, tablet or TV into a scrollable sign for welcome messages, timers or Wi-Fi passwords, no app needed.

## Security, Privacy & Curiosities

* [**Eye of Sauron: Long-Range Hidden Spy Camera Detection and Positioning with Inbuilt Memory EM Radiation**](https://www.usenix.org/conference/usenixsecurity24/presentation/zhang-qibo) - USENIX Security paper on spotting hidden cameras through their memory emissions.
* [**Man discovers his parents' coffee machine used 1TB of data in 10 days**](https://www.dexerto.com/entertainment/man-discovers-his-parents-coffee-machine-used-1tb-of-data-in-10-days-3416399/) - A reminder to check what the smart appliances are really uploading.
* [**Fake Meeting**](https://fakemeeting.app/) / [**Virtual Meeting Simulator**](https://z.tools/t/fake-meeting) - Browser tools that simulate a video call with camera, mic and screen sharing, for looking busy on demand.
* [**Subastas judiciales de inmuebles en España | Pujarr**](https://pujarr.com/) - All the property auctions from the BOE, the tax agency and the social security system on one map, with starting prices and charges.
