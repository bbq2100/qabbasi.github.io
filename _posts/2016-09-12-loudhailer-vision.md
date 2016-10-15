---
layout: post
title: LoudHailer – Reaching your Audience
excerpt: "Building the next fancy Goldberg machine just for learning purposes convinced myself fairly quickly.
          That said, I started this blog series to document my learn achievements during this side project..."
categories: [Loudhailer]
comments: true
---

### What's this?
Building the next fancy [Goldberg machine](https://en.wikipedia.org/wiki/Rube_Goldberg_machine) _just_ for learning purposes convinced myself fairly quickly.
That said, I started this mini blog series to document my learn achievements during this side project.
Originally I started to write one monolithic post and then changed my mind and chose to destruct it into three consumable parts.

For the curious: the illustrated `code` in the subsequent posts can be found [here](https://github.com/qabbasi/Loudhailer).
Also, for any remarks or suggestions on the project I'm always grateful!

### The idea
What's LoudHailer about? Functionally it's a voice recognition app to detect emergency cases.

![Vision](http://i.imgur.com/CvWgRl0l.png) 

Technically spoken it's a stream processing application based on [Akka Streams](http://akka.io) and consists of the actual voice recording and a processing backend,
which automatically detects alarming words and notifies clients about an incident. For this I created a tiny Android app using [Kotlin](http://kotlinlang.org).
Also to make it super duper easy to use, I dockerized LoudHailer to run it directly on a [Raspberry](http://blog.hypriot.com/getting-started-with-docker-on-your-arm-device/). Cool, huh?

### Next
Let's get to the building blocks! Starting with [functional stream processing]({% post_url 2016-09-12-loudhailer-vision %}) using Akka Streams.