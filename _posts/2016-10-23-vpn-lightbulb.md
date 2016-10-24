---
layout: post
title: "Useful hacking with the Internet of Shitty Things"
date: 2016-10-23 12:05:00 +0100
author: HeadCrash
categories: thinks internet-of-shitty-things vanity
---

# Hacking on the Internet of Shitty Things with purpose

> Riding on the coat tails of the mirai hack that used insecure Internet of Shitty Things devices as an attack vector we thought we'd see what sort of useful hacking we could do with a cheap shitty RGB IoT lightbulb.

!["Bang!"](http://media.fuckyou.computer/exploding-bulb.gif)

We decided on the LifX range of RGB LED bulbs for the simple reason that it was the first set of IoT bulbs that was hacked remotely, they
don't rely on a hub and they, like me, are cheap. In their defense the firmware has already been patched but I imagine that all the negative press due to the hack hasn't done their sales too much good. Still, it appears as though they're still in the game and after reading through their documentation I can't fault their dedication to security. If we weren't completely disregarding the EULA expressly to hack the machines to do our bidding then I'd be tempted to use their nice little API for doing stuff at home.

## Links
* ["That LifX Smart Lightbulb Hack Wasn't Easy"](https://securityledger.com/2014/07/that-lifx-smart-lightbulb-hack-wasnt-easy/)
* ["Controlling Lights With BASH"](https://community.lifx.com/t/controlling-lights-with-bash/31/4)
* ["CMD Line Tool for LifX"](https://github.com/MichaelAquilina/lifx-cmd)
* ["Hacking Into Internet Connected Light Bulbs"](https://www.contextis.com/resources/blog/hacking-internet-connected-light-bulbs/)
