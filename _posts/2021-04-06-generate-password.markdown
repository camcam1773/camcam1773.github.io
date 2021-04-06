---
layout: post
title:  "Generate Password with Random Characters"
categories: linux tips
---

```
$ pwgen -1s 32
```

This command above generates a 32-character secure random password consisting of upper/lowercase characters and numbers. You can change 32 to any number you like.

```
$ openssl rand -base64 32
```
It is also poosible to do the same with openssl rand function. However, in this case number represents bytes not the amount of characters.

I should also mention that these commands are not always available by default. But it should be possible install with your package manager like apt-get, yum etc.