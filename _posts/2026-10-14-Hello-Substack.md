---
title: Hello Substack!
description: "Hello Substack! I'm mirroring my content from AnonJr.com to Substack, as well as making sure there's a Substack presence for Bible By Example."
date: 2026-10-14 16:30:00
tags:
    - Bible By Example
    - Meta
    - Projects
    - Programming
repost: ""
---

Hello Substack! After spending a fair amount of time lurking on Substack, and trying to figure what's next for AnonJr.com, I've decided to mirror the past and future content. It's not a move, I firmly believe in retaining final ownership of your content and keeping it in a place you control. [AnonJr.com][1] will remain the canonical home of my writing, videos, etc., though the [AnonJr Substack][2] will now hold a copy so that I can add support for [Games Revisited][3] and other projects as well as allowing for comments and discussion. And hopefully better circulation.

<!--more-->

I've toyed with various comment systems in the past, and at this juncture I'd rather just leave the bulk of what's needed to manage it to Substack. I've run forums (kids, ask your parents) and don't relish working on anti-spam code again. Most of the other systems seem to either clutter my GitHub repo or require me to trust that no one is going to inject anything into the JavaScript includes. Sure. Because that's never been an issue.

No matter what comment system I used, it doesn't really matter if there's no real traffic. The internet has contracted again. We went from the small walled gardens of AOL and similar services to a wide array of personal websites, back to consolidating around Medium, Substack, Facebook, and such. It's in some ways more than before, but if you want to find people you can't really run solo anymore.

## Introductions and Reintroductions

Who and what I am

## Migrating

As I said in the intro, I believe in keeping all my content in a place I control. I've been around long enough to know that at some point Substack will either dwindle or become a place I don't want to be at anymore. I've already [made a feed specific to Dev.to][4], stayed there for a while, and then let it quietly go by the wayside.

This time it's a little different. First, I need to move *everything*, not just select posts. Second, I want to make sure this is something I can use later if I need to move again.

I don't like doing the same work again, so I asked the [Council of LLMs][5] to steel-man the case for altering the Atom feed code I already had from a previous iteration of AnonJr.com and steel-man the case for a new RSS 2.0 implementation. In the end I went with making an RSS 2.0 implementation.

After some frustration, and consultations, I got something working in the end. The [full code][6] for `content_migration.xml` is up on GitHub, but I want to highlight a couple things in case it's of use for someone else.

Notably, I have an inordinate love for ellipses. Particularly in several titles. Apparently Substack doesn't HTML render the titles, but makes them proper encoded text. So I had to fix a few pages post-import. The code now has the following to prevent that from happening in the future:

{% highlight liquid %}
{% raw %}<title>{{ post.title | replace: '&hellip;', '…' | xml_escape }}</title>
<link>{{ post.url | absolute_url }}</link>
<guid isPermaLink="true">{{ post.url | absolute_url }}</guid>
<pubDate>{{ post.date | date_to_rfc822 }}</pubDate>{% endraw %}
{% endhighlight %}

There doesn't appear to be an easy way to represent post tags in any RSS format, but the general recommendation I could find was to flatten categories and tags into `<category>` elements. I'm not using Jekyll Categories right now, but I figured I'd add it now so it's there if I need it in the future.

{% highlight liquid %}
{% raw %}{% for category in post.categories %}
<category><![CDATA[{{ category }}]]></category>
{% endfor %}

{% for tag in post.tags %}
<category><![CDATA[{{ tag }}]]></category>
{% endfor %}{% endraw %}
{% endhighlight %}

Highlighting why I've settled on using a Council over one particular LLM over another: I asked if Substack's Import tool would add tags and one said "yes", another said "no", and the third said "maybe". Well that about covers all the bases. Spoiler alert: it didn't import mine. Adding tags to 711 posts was less than fun. At least it gave me the opportunity to make sure nothing else was mangled in the import. Other than a missing YouTube embed and some of the aforementioned &amp;hellip; issues everything seems to have imported correctly.

## Games Revisited

One of the nice side effects of going through all 711 posts to add tags was a chance to skim the history of projects that fell behind.

As much as I liked [The 47%][7], I'm willing to let that one rest. World of Tanks in particular, and Wargaming in general, became something I just don't want to interact with anymore. I do miss having a decent game to jump in, platoon with some friends, and just play. Just play, shoot, have fun. I need to find another game like that. I never did post them here or to YouTube, but I did try Battlefield V for a while and streamed it. Let's just say I'm too far out of practice for a shooter like that. I got left behind somewhere along the way.

I also realize that I miss the main bread and butter of [Games Revisited][3] - a weekly live stream that got cut into shorter episodes that rolled out through the week on YouTube. Notably, I really need to finish [The Legend of Zelda: A Link to the Past][8]. I left that one hanging during a particularly rough depressive episode and then my cancer journey put *everything* on pause for a while. If you've never poked around there's some good seasons and some other seasons. The [Trine/Trine 2 series][9] I did with my middle sister and her husband was a lot of fun. The [Chrono Trigger][10] series was very nostalgic, though a little rough as it was an early season before I really settled into the format.

Once I get a trailer for Bible By Example set up and the last few bits with that done I'll get back to Games Revisited. There's been some hardware changes between then and now, and I need to finish the move from XSplit to Streamlabs Desktop (I think that's what it's called now - I keep thinking of it as "Streamlabs OBS/SLOBS" but that probably makes me old and wrong). Once that's done I'll finish up the Link to the Past season and see what I have floating around that would make for a good Season 09.

BTW: While I was writing this I noticed there wasn't a clean way to link to a tag page generated by `jekyll-archives` other than hard-coding the link and hoping the tag doesn't change (e.g. fixing a typo) and break the link. So I went on a two-day yak shaving fest to build a custom plugin. I'll have to write that one up next.
{: .notice--info}

## Bible By Example

Its own Substack. Goals and aspirations. Borders between what faith posts will appear here vs there.

## Conclusion?

Close it out.

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
