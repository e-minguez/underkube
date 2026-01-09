---
aliases:
- /posts/2019-06-18-firewalld_tips_and_tricks/
categories:
- tech
date: 2019-06-18 17:19:08+02:00
draft: false
slug: firewalld_tips_and_tricks
tags:
- firewalld
- tips
title: Firewalld tips & tricks
---

# Show all rules

```
sudo firewall-cmd --list-all
```

# Redirect ports

```
sudo firewall-cmd --zone="$(firewall-cmd --get-default-zone)" \
  --add-forward-port=port=443:proto=tcp:toport=8443 --permanent
sudo firewall-cmd --zone="$(firewall-cmd --get-default-zone)" \
  --add-forward-port=port=80:proto=tcp:toport=8080 --permanent
```