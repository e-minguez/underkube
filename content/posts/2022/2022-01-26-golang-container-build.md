---
aliases:
- /posts/2022-01-26-golang-container-build/
categories:
- tech
date: 2022-01-26 08:30:00+00:00
description: Quick and dirty way to compile a golang binary using a container
draft: false
slug: golang-container-build
tags:
- golang
- podman
title: Quick and dirty way to compile a golang binary using a container
---

I wanted to compile the hypershift binary but it requires golang 1.17 which is not included in Fedora 35, so I ended up doing this:

```
mkdir ./tmp/ && \
  podman run -it -v ${PWD}/tmp:/var/tmp/hypershift-bin/:Z --rm docker.io/golang:1.17 sh -c \
    'git clone --depth 1 https://github.com/openshift/hypershift.git /var/tmp/hypershift/ && \
    cd /var/tmp/hypershift && \
    make hypershift && \
    cp bin/hypershift /var/tmp/hypershift-bin/' && \
    cp ${PWD}/tmp/hypershift ~/bin/
```

HTH