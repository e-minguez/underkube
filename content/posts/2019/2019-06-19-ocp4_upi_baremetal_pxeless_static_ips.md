---
aliases:
- /posts/2019-06-19-ocp4_upi_baremetal_pxeless_static_ips/
categories:
- tech
date: 2019-06-19 15:16:45+02:00
draft: false
slug: ocp4_upi_baremetal_pxeless_static_ips
tags:
- ocp4
- openshift
title: OCP4 UPI baremetal pxeless with static ips
---

Do you want to deploy an OCP4 cluster without using PXE and using static IPs?

I've got you covered. See [my unsupported step by step instructions](https://github.com/e-minguez/ocp4-upi-bm-pxeless-staticips) on how to doing it,
including:

* No PXE (pretty common scenario in big companies)
* Avoid installing stuff and use containers instead (instead yum/dnf install httpd, haproxy,... use containers)
* Use rootless containers if possible
* Use Fedora29/RHEL8 stuff (nmcli, firewalld, etc.)

Enjoy!