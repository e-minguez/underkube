---
aliases:
- /posts/2014-11-25-set-file-as-executable-in-svn/
categories:
- tech
date: 2014-11-25 09:52:31+00:00
draft: false
slug: set-file-as-executable-in-svn
tags: []
title: Set file as executable in svn
---

`chmod` doesn't do the trick, so you need to set the proper flag in svn with:

```
svn propset svn:executable ON <filename>
```