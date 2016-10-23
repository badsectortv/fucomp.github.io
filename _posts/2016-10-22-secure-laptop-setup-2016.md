---
layout: post
title: "Thoughts on a 2016 secure laptop OS build"
date: 2016-10-22 14:05:00 +0100
author: HeadCrash
categories: thinks self-help
---

# Thoughts on a 2016 secure laptop OS build

> Secure By Default?

!["No Entry"](http://media.fuckyou.computer/locked_door.gif)

We've previously covered a potential way of keeping yourself secure with obsolescence but how does one protect oneself in today's happy-hacking world of the internet with modern techniques and modern tools?

I've recently had the opportunity to start from scratch on one of my main computers and thought I would take the time to consider my options.

## Considerations

I want to keep the base OS as Mac OS, up-to-date but with very little actually installed on it for speed and security. It will be encrypted by default.

## Ideas
* Containers / Separation of concerns
* Encryption
* Honeypots

## VMs
I initially think that I would run some VirtualBox VMs to do my work in but space becomes a major issue quickly due to the virtual hard drives. I've since moved onto the idea of Docker containers as it's possible to spin up new environments from a single parent. Think of them in the same way that GIT works but for virtual machines. The initial image can be kept up-to-date easily which will then propagate through the image clones for added security.

## Links
[docker.com](https://www.docker.com/)
