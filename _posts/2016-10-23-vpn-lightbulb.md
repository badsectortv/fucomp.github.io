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

We decided on something like the [Northtime](http://gzyigang.en.made-in-china.com/product/pvtQfKqJJFcU/China-Rgbww-RF-WiFi-LED-Dimmable-Remote-Controller-LED-Bulb.html) RGB LED bulb for the simple reason that although it was not the first set of IoT bulbs that was hacked remotely, they don't rely on a hub and they, like me, are cheap. Also another consideration was that the cheaper the unit we could find would probably have less stringent security.

I did some preliminary research into [LifX](http://www.lifx.com/), even going so far as to install and decompile their Android app which was interesting for several reasons but after their recent wifi password hack they've beefed up their already substantial security to put it out of reach of a simple amateur.

## Further Reading
* [That LifX Smart Lightbulb Hack Wasn't Easy](https://securityledger.com/2014/07/that-lifx-smart-lightbulb-hack-wasnt-easy/)
* [Controlling Lights With BASH](https://community.lifx.com/t/controlling-lights-with-bash/31/4)
* [CMD Line Tool for LifX](https://github.com/MichaelAquilina/lifx-cmd)
* [Hacking Into Internet Connected Light Bulbs](https://www.contextis.com/resources/blog/hacking-internet-connected-light-bulbs/)
