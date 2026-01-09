---
aliases:
- /posts/2014-09-11-run-a-process-in-background-nohupped-and-without-nohup-out/
categories:
- tech
date: 2014-09-11 14:12:06+00:00
draft: false
slug: run-a-process-in-background-nohupped-and-without-nohup-out
tags:
- background
- linux
- nohup
- tips
title: Run a process in background, nohupped and without nohup.out
---

```
nohup yourprocess >/dev/null 2>&1&
```