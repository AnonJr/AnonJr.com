---
title: Hello Substack!
description: "Hello Substack! I'm mirroring my content from AnonJr.com to Substack, as well as making sure there's a Substack presence for Bible By Example."
date: 2026-10-15 15:20:00
tags:
    - Bible By Example
    - Meta
    - Projects
    - Programming
repost: ""
---

Hello Substack! After spending a fair amount of time lurking on Substack, and trying to figure out what's next for AnonJr.com, I've decided to mirror past and future content. It's not a move - I firmly believe in retaining final ownership of your content and keeping it in a place you control. [AnonJr.com][1] will remain the canonical home of my writing, videos, etc.

<!--more-->

![Hello Substack](/assets/img/2026-10-15_HelloSubstack.svg)

The [AnonJr Substack][2] will now hold a copy so that I can add support for [Games Revisited][3] and other projects as well as allowing for comments, discussion, and (hopefully) better circulation.

I plan on doing some proper writing again, so look for stuff on programming and tech, guitars and luthiery, and some writing on faith. I'm sure I should be siloing those out to separate Substacks for maximal subscribership, but I think we lose something in discouraging authors from showing their wider interests.

I'm looking for comments too. I've toyed with various comment systems in the past, and at this juncture I'd rather just leave the bulk of what's needed to manage it to Substack. I've run forums (kids, ask your parents) and don't relish working on anti-spam code again. Most of the other systems seem to either clutter my GitHub repo or require me to trust that no one is going to inject anything into the JavaScript includes. Sure. Because that's never been an issue.

No matter what comment system I used, it doesn't really matter if there's no one reading, and hopefully Substack's recommendation system will help with that. The internet has contracted again. We went from the small walled gardens of AOL and similar services to a wide array of personal websites, back to consolidating around Medium, Substack, Facebook, and such. It's in some ways more varied than before, but if you want to find and be found by people you can't really run a solo website anymore.

## Introductions and Reintroductions

With such a long lull on the main site, and a new Substack presence, it seems the perfect opportunity to do a little (re)introduction.

The recently updated "About" page is finally closer to something worth using. I am shy, and I much prefer to be the man behind the curtain than the one on stage, so writing those sorts of things is just a tough thing for me. Besides, who am I? My job? My education?

I am a Christian. I am a life-long learner. I tend towards the "Jack of all Trades" sort of thing - the full quote, not the misleading fragment everyone remembers. I like understanding how things work, and from first principles, which is why I like building things.

My degree is in Computer Programming and I even worked in the field I majored in! I was the guy who wrote and maintained the software that ran online training for staff at a mid-sized hospital. And copy edited the content. And provided the technical support to management and staff. Also (huh, wonder why I burned out), being in the Training and Development department, I had "other job duties as assigned" that included running various classroom training for staff too. At least that wasn't new - I'd coached my sister's rec soccer team in high school, and taught Lifeguarding, swimming, and was an assistant swim coach in college.

I love music, I play around with guitar (I am **not** good enough to call myself a guitarist), and I've even worked as a strings repair tech. Technically I could refer to myself as a luthier, though I think I'm missing a couple skills to feel comfortable claiming the title.

I did a fair amount of writing in college, and some for work as well - though most of that was for the hospital and unsuitable for general publishing. I've promised myself a return to writing several times throughout the life of this site, and yet it seems to die not long after. A big part of that was the impact of burnout and the depression that came along with it. It's only after skimming the full 711 post library that I can see just how it hindered things. At least now I've actually sought help and made real changes. Perhaps I'll write about that later, not sure I'm quite at that point just yet.

## Making the Move

I've been around long enough to know that at some point Substack will either dwindle or become a place I don't want to be at anymore. I've already [made a feed specific to Dev.to][4], stayed there for a while, and then let it quietly go by the wayside.

This time it's a little different. First, I need to move *everything*, not just select posts. Second, I want to make sure this is something I can use later if I need to move again. I worked with the [Council of LLMs][5] to make an RSS 2.0 feed for all existing posts that should be usable if I mirror anywhere else too. The [full code][6] for `content_migration.xml` can be viewed on GitHub, and I may do a more technical post in the future, but for now I want to highlight a couple things in case it's of use for someone else.

Notably, I have an inordinate love for ellipses. Particularly in several titles. Apparently Substack doesn't HTML render the titles, but makes them proper encoded text. So I had to manually fix a few pages in Substack after importing, and I added a little extra code to make sure it's not a problem in the future.

There doesn't appear to be an easy way to represent post tags in any RSS format, but the general recommendation I could find was to flatten categories and tags into `<category>` elements. Highlighting why I've settled on using a Council over one particular LLM over another: I asked if Substack's Import tool would add tags and one said "yes", another said "no", and the third said "maybe". Well that about covers all the bases. Spoiler alert: it didn't import mine. Adding tags to 711 posts was less than fun. At least it gave me the opportunity to make sure nothing else was mangled in the import.

Other than a missing YouTube embed and some of the aforementioned &amp;hellip; issues, everything seems to have imported correctly.

## Games Revisited

One of the nice side effects of going through all 711 posts to add tags was a chance to skim the history of projects that fell behind.

As much as I liked [The 47%][7], I'm willing to let that one rest. World of Tanks in particular, and Wargaming in general, became something I just don't want to interact with anymore. I do miss having a decent game to jump in, platoon with some friends, and just play. Just play, shoot, have fun. I need to find another game like that. I never did post them here or to YouTube, but I did try Battlefield V for a while and streamed it. Let's just say I'm too far out of practice for a shooter like that. I got left behind somewhere along the way.

I also realize that I miss the main bread and butter of [Games Revisited][3] - a weekly live stream that got cut into shorter episodes that rolled out through the week on YouTube. Notably, I really need to finish [The Legend of Zelda: A Link to the Past][8]. I left that one hanging during a particularly rough depressive episode and then my cancer journey put *everything* on pause for a while. If you've never poked around there's some good seasons and some other seasons. The [Trine/Trine 2 series][9] I did with my middle sister and her husband was a lot of fun. The [Chrono Trigger][10] series was very nostalgic, though a little rough as it was an early season before I really settled into the format.

Once I get a trailer for Bible By Example set up and the last few bits with that done I'll get back to Games Revisited. There's been some hardware and software changes between then and now that need to be addressed, and once that's done I'll finish up the *Link to the Past* season and see what I have floating around that would make for a good Season 09.

BTW: While I was writing this I noticed there wasn't a clean way to link to a tag page generated by `jekyll-archives` other than hard-coding the link and hoping the tag doesn't change (e.g. fixing a typo) and break the link. So I went on a two-day yak shaving fest to build a custom plugin. I'll have to write that one up too.
{: .notice--info}

## Bible By Example

Another thing I noticed while reviewing the imported posts is the intermittent references to work on [Bible By Example][11] - a podcast I've long had a desire to do, and am now finally nearing release. It's also going to have [its own Substack][12] with all the content mirrored there as well. Like with AnonJr.com I want a central authoritative hub for all my content that I have control over, but I also want to make the content as accessible as I can.

Unlike other projects I do under the "AnonJr.com" banner, I want to keep this one separate. Where CoffeeCraft, Games Revisited, or even the other writings I have and will put on AnonJr.com are more focused on my opinions and views, Bible By Example is going to focus more on the plain meaning of scripture - regardless of what I think - and a look at the Overton Window of generally accepted belief where Christian traditions vary, drawn from commentaries with a spectrum of views and other helps. There will be a little of my opinion here and there, it's unavoidable. But I will keep that to a minimum and work hard to be clear when something presented is my opinion vs what's a reasonable reading or within the spectrum of orthodox belief.

In addition to the podcast episodes and links to various options for listening, I'll post some articles mostly focused on deeper dives into archeology, language, and other related areas with the goal of supporting and enhancing an understanding of what the Bible is, what it isn't, how we got it, why Christians consider it reliable, and what the peshat is. I won't engage in heavy apologetics on Bible By Example, though there will be a natural undercurrent in working through the material.

The heavy apologetics I'll post here on AnonJr.com. 😉

I see a lot of old heresies in new dress floating around, a lot of old debunked theories floating around like some sort of intellectual background radiation, and some subtle attacks on Christian fundamentals - all of which deserve reply.

I plan on doing a longer "Road to Bible By Example" series, probably on the Bible By Example side of things, giving a little more history and background.

## Conclusion

Now that I've finished migrating the old content, I'll resume developing a program to automate publishing to both [AnonJr.com][1] and [the AnonJr Substack][2] without requiring me to copy/paste and fix, and it will do the same for Bible By Example. [Games Revisited][3] should be resuming soon, and the work on [Bible By Example][11] should be finished in time for a launch within the next two weeks.

Here's looking for more, and more regular writing.

[1]: https://www.anonjr.com/
[2]: https://anonjr.substack.com/
[3]: {% link _pages/gamesrevisited.md %}
[4]: {% post_url 2018-11-04-Special-Feed-for-Dev.to %}
[5]: {% post_url 2026-08-21-Council-of-LLMs %}
[6]: https://github.com/AnonJr/AnonJr.com/blob/master/_pages/content_migration.xml
[7]: {{ "The 47%" | tag_url | relative_url }}
[8]: {{ "The Legend of Zelda: A Link to the Past" | tag_url | relative_url }}
[9]: {{ "Trine" | tag_url | relative_url }}
[10]: {{ "Chrono Trigger" | tag_url | relative_url }}
[11]: https://www.biblebyexample.com/
[12]: https://biblebyexample.substack.com/
