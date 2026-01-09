---
aliases:
- /posts/2014-09-16-simple-command-to-create-a-timelapse-from-a-few-images/
categories:
- tech
date: 2014-09-16 18:23:46+00:00
draft: false
slug: simple-command-to-create-a-timelapse-from-a-few-images
tags:
- ffmpeg
- timelapse
- tip
title: Simple command to create a timelapse from a few images
---

```
cat *jpg* | ffmpeg -f image2pipe -r 30 -vcodec mjpeg -i - -vcodec libx264 out.mp4
```