---
aliases:
- /2007/11/28/purgar-los-paquetes-desinstalados-en-debian/
author: minwi
categories:
- linux
- tech
date: 2007-11-28 10:39:01+00:00
draft: false
slug: purgar-los-paquetes-desinstalados-en-debian
tags:
- debian
- sysadmin
title: Purgar los paquetes desinstalados en Debian
type: post
---

dpkg --purge $(dpkg --get-selections | grep deinstall|cut -d" " -f1)

Easy! :D