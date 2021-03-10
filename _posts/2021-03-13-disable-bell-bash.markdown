---
layout: post
title:  "Disable bell/beep on terminal"
date:   2021-03-14 12:00:00 +0100
categories: linux tips
---

If you wanto to disable the bell/beep sound that occurs when pressing TAB etc., add *set bell-style none* to .inputrc file in your home directory. 
If it doesn't exist, you can just create one.
You need to log out and then log in to your shell in order for this to be applied. 

This bash command should do trick:
```bash
echo "set bell-style none" >> ~/.inputrc
```