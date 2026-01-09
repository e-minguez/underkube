---
aliases:
- /posts/2014-11-19-package-dependency-graph-of-any-installed-rpm-package/
categories:
- tech
date: 2014-11-19 14:42:01+00:00
draft: false
slug: package-dependency-graph-of-any-installed-rpm-package
tags: []
title: Package dependency graph of any installed RPM package
---

Vía http://xmodulo.com/check-rpm-package-dependencies-fedora-centos-rhel.html:

* Just install rpmorphan and graphviz:

```
yum install -y rpmorphan graphviz
```

For example, for gzip package:

```
rpmdep.pl -dot gzip.dot gzip
dot -Tpng -o output.png gzip.dot
```

Browse the output.png file and it should looks like:
![graph dependencies](https://farm4.staticflickr.com/3918/14453050980_53de4e8277_z.jpg)