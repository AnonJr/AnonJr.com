---
title: "A Pretzel, A Jekyll, Some Pages, and a Cranky Git"
description: "Restarting some projects, and building some sites using Jekyll, Pretzel, and GitHub Pages."
date: 2017-07-28 13:00:00 -0500
author: AnonJr
layout: post
comments: true
tags:
- meta
- projects
---

Don't mind the dust, and sorry about the cobwebs&hellip; To say it's been a while would be something of an understatement since the last post is from 2013.

At the time I was earnestly looking to ramp up and do something with the Blogger account I opened and never actually used for anything other than oAuth. Life hit hard - a combination of events, accumulated effects of a sleep disorder, depression, and the early stages of burnout - and so it sat a little longer.
<!--more-->
I've made a few halfhearted attempts to start it all back up, but as you can clearly see nothing came to much. So here we are.

{% embed youtube "Tkfjrp0PNYw" %}{% endembed %}
<!-- https://youtu.be/Tkfjrp0PNYw -->

> If you've managed to make it this long without watching the awesome (and canceled too soon) show Firefly, get your popcorn and streaming service of choice going and enjoy a weekend binge. We can even compare notes with the good folks at [Cordkillers](http://www.cordkillers.com/).

So what now? I’m trying to get a few projects lined up:

* I’m almost done rebuilding a few of my websites – this being one of them.
* I’m developing a podcast, one I hope to be able to eventually turn into a small income stream.
* I’m restarting work on a campaign setting I was building with my sister and her husband.
* I’m (re)starting work on two novels rooted in the above campaign setting. I’d love for both the game and the books to become something awesome and synergistic – I’ll gladly settle for one or the other taking root. I like the world we’re building and I just want to play in it. :)

My goal is to get one or more of these up to enough of an income to cover the bills, and do something different for a while. The various issues creating drag in my life certainly don't help, but rather than dwell on that let's look at the actual focus of the title.

Most of my programming work has been in medium-scale CMSs - something that is *way* overkill for a site like this, the podcast site, and a few other projects. So I joined along the static site generator bandwagon and picked a couple to play with.

This site is using [Pretzel](https://github.com/Code52/pretzel/), a .NET tool that's compatible with the templates and whatnot used by the Ruby-based [Jekyll](http://jekyllrb.com/). Since I do most of my work and play on Windows, it seemed like the perfect fit. Especially since (at the time) trying to get Ruby anything running on Windows was a bit of a pain.

I've found a few areas where the templating and Liquid commands don't *quite* fit, but it's been fairly straight forward. Given my preferences, I do like that Pretzel uses LESS instead of SASS. If there was a little more active development, I'd heartily recommend it.

The podcast site ([incompletly up](http://www.biblebyexample.com) as of writing this) is using the aforementioned Jekyll. When I'd finally mustered enough energy to get cracking on this project, installing Ruby and Jekyll on Windows became significantly less painful. And as long as you're willing to do a little work with the setup, WSL has made it even easier.

I managed a little more traction and rapid progress on the latter since I was more willing to grab [a theme that someone else had put together](https://mmistakes.github.io/minimal-mistakes/).

Both projects are up on GitHub, and are being hosted using GitHub pages. Now that's been an interesting endevour&hellip; particularly getting the domains squared away. The next step for both sites will be to get them behind [Cloudflare ](https://www.cloudflare.com/) for some CDN goodness and HTTPS.

I'll write a little more about each project individually, and some "thinking out loud" type posts over the next few days.