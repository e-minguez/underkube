---
aliases:
- /2007/12/02/backup-de-time-machine-en-una-unidad-samba/
author: minwi
categories:
- apple
- backup
date: 2007-12-01 22:06:50+00:00
draft: false
slug: backup-de-time-machine-en-una-unidad-samba
tags: []
title: Backup de time machine en una unidad Samba
type: post
---

No hace falta hacer nada más que escribir en terminal lo siguiente:

CODE
defaults write com.apple.systempreferences TMShowUnsupportedNetworkVolumes 1

Al hacerlo, aparecerá el AirDisk o Samba como destinos de Time Machine.

Copy & paste de [macuarium](http://www.macuarium.com/foro/index.php?showtopic=231988&st=25#)