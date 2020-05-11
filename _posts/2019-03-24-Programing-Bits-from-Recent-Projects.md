---
title: "Programming Bits from Recent Projects"
description: "Reviewing the work on recent projects, and noticing a few things."
date: 2019-03-24 23:30:00 -0400
tags:
- meta
- programming
- CoffeeCraft
repost: "dev.to"
---

I've got the first live stream for [CoffeeCraft](https://www.coffeecraft.us/) coming up this Monday at 7pm EDT (-4 UTC? I think? I hate Daylight Saving). I did a [test stream](https://www.coffeecraft.us/2019/03/Test-Stream.html) a while back, and [downloaded some music](https://www.coffeecraft.us/2019/03/AnonJr-Live-Playlist-v1.html) to run in the background. I've got a plan and now I need to burn off some nervous energy. There's probably a whole other post in there but I spent too much time today finding stuff to do instead of writing the stuff that was on my mind. With a little more work I'll get the nervous slacking to actual writing ratio tipped in the other direction. :smiley:
<!--more-->
>Side note: before I get too far away from the impending live stream, since this is the beginning of the channel I don't really expect much in the way of attendance - so, if you'd like to hop in chat and ask some programming or career questions I'd be more than happy to answer. I'm no tech luminary like Scott Hanselman or Troy Hunt, but I've got 14 years of doing actual work managing systems for a mid-sized health system. I might have a nugget or two worth sharing.

So, if that's not this post, what is? This post is a sort of follow up from my [Projects Update]({% post_url 2019-03-22-Projects-Projects-Projects-Updates %}) post. And a chance to burn off some nervous energy&hellip; starting something is, well, something.

## AnonJr.com
The [GitHub repo](https://github.com/AnonJr/AnonJr.com) is available in all its beauty and horror. Like other projects I and every other human have worked on, present-me is embarrassed about some of the things past-me thought awfully clever. That's ok. I'm sure future-me will also be shaking his head about something that I'm currently sure is awesome.

First commit after things started settling down was to add the [Dev.to](https://dev.to/) link as a part of a general update on the sidebar. Funny thing is, not long after the commit [@benhalpern](https://twitter.com/bendhalpern) posted this reminder:

<blockquote class="twitter-tweet" data-lang="en"><p lang="en" dir="ltr">Reminder to put the DEV badge on your personal site alongside Twitter and your other social links. You can either use the SVG or Font Awesome.<a href="https://t.co/itCHG96NX8">https://t.co/itCHG96NX8</a><br><br>Happy coding ❤️</p>&mdash; Ben Halpern 🤗 (@bendhalpern) <a href="https://twitter.com/bendhalpern/status/1099410983695478784?ref_src=twsrc%5Etfw">February 23, 2019</a></blockquote>
<script async src="https://platform.twitter.com/widgets.js" charset="utf-8"></script>

Fun thing when doing projects like this - you find out what other libraries are out of date. :confused:

After a bit of "did I do that right?" style double-checking source, output, references, and such it turned out I hadn't updated [Font Awesome](https://fontawesome.com/) in a while. Also turns out they've got an easier way to use the library, but I'll get to that one next. For AnonJr.com I continued using the [self-hosting method](https://fontawesome.com/how-to-use/on-the-web/setup/hosting-font-awesome-yourself). For new projects I wouldn't recommend doing this unless you had a clearly articulatable reason why you *needed* to host those files yourself - e.g. "the project is running internally on the company LAN, and staff won't have access to external resources". That's what I had to do when working at Cape Fear Valley, as some staff had no access to resources external to the corporate network. As for here I wasn't up to ripping everything up and re-working that bit of styling for two icons. I'll save that for the move from Pretzel to Git.

A few days later I set to updating the project links on the sidebar, and realized I really needed to update the pages and add a couple others. It was rather nice to upgrade all the links to HTTPS and check off a goal that you'll see mentioned in quite a few previous posts. It was also nice to add a few logos and tighten up the copy, and a little sad to reflect on some of the neglected projects. If there's a key takeaway for this note, it's take some time to look over your past projects and work, and reflect. Marvel at the growth you've made, and groan at the things you see you still need to work on. If you haven't seen growth, or think there's no growth needed, then you might want to reflect on that.

There's a couple other commits in there, but the only one worth a mention is adding a proper Favicon and getting the images and meta information set up for Twitter/Facebook/etc. to render a proper card. It amazes and frustrates me that we have to add so many icon links because of the wide variety of devices. I could see maybe a "large" and a "low bandwidth" version, but because iPhone needs one size, and iPad needs another, and Windows will pin a site but only with a third size, and so on - I now have 8 or so different size icons floating around. Not to mention Twitter would rather one set of meta tags for a card, but Facebook uses another&hellip; I'd recommend a common standard, but we'd probably be looking at the usual XKCD comic.

![XKCD Standards](https://imgs.xkcd.com/comics/standards.png)

## CoffeeCraft.us
This is the [other repo](https://github.com/AnonJr/CoffeeCraft.us/) that has taken up most of my commits in the last few months. I'd like to present some interesting technical challenges, but mostly it was wrestling with content, layout, and design. I started with [MMistakes "So Simple" theme](https://github.com/mmistakes/so-simple-theme), and started building from there.

I won't speak for anyone else on this one - for me one of the struggles on this project (and the others I'm working on) is I'm both designer and client. For some reason, despite the ability to make amazing things I can't seem to make amazing things *for me*. Look at the history. Look at all the parts I waffled on. I even have "**Adding search, updated text ... and feeling lost**" as a commit message.

## Wrapping it up
Ok, so that wasn't as technical as it seemed when I first sat down to write&hellip; and as much as I love using [Ghostewriter](https://github.com/wereturtle/ghostwriter) to compose posts, I find it immensely frustrating that the cursor blinks even when the program doesn't have focus - so I've started typing the next sentence in the address bar and done all sorts of funky other things as the thing that actually had focus suddenly started getting random letters and returns. Before I get too frustrated I'll see if I missed an update.

I stayed up far later than I'd originally intended, so I'll cut this one short. I've got to be up for work at 4am&hellip; and an impending live stream at 7pm EDT. I'll close with a reminder that since this is the beginning of the channel I don't really expect much in the way of attendance - so, if you'd like to hop in chat and ask some programming or career questions I'd be more than happy to answer. I'm on [Twitch](https://www.twitch.tv/anonjr_live), [Mixer](https://mixer.com/AnonJr_Live?vod=91997262), and [YouTube](https://www.youtube.com/channel/UCXafqhKHbkSUIrq0LAuu0tw) - use the one you feel most comfortable with. [Restream.io](https://restream.io/) should be syncing the chat between all the channels, and I'll have their chat app up and running (it's supposed to show me all the chats as they go across).

Hope to see you there.