---
aliases:
- /posts/2014-12-03-spacecmd-issues-and-cache/
categories:
- tech
date: 2014-12-03 12:13:22+00:00
draft: false
slug: spacecmd-issues-and-cache
tags: []
title: spacecmd issues and cache
---

When using spacecmd, it caches stuff like systems and packages.
If you are doing operations like register and delete systems, maybe it's useful to delete the cache if there are messages like:

```
ERROR: redstone.xmlrpc.XmlRpcFault: No such system - sid = 1000010740
```

To clear cache, use:

```
spacecmd clear_caches
```