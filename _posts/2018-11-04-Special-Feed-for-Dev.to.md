---
title: "Special Feed for Dev.to"
description: "Built a special RSS feed for the posts I want to send over to Dev.to"
date: 2018-11-04 22:30:00 -0500
author: AnonJr
layout: post
comments: true
repost: "dev.to"
tags:
- meta
- programming
---

Back in January 2017 I started following what looked like a small and promising community of programmers (and those in adjacent fields) over at [Dev.to](https://dev.to/). At the time I had the site's whole feed pumping into my Feedly list, I'd commented on a few posts, and I was starting to think about either revitalizing this blog or picking some other platform for posting.

In the end I decided to try and revitalize this site, beginning with [a bit on the tech]({% post_url 2017-07-28-A-Pretzel-A-Jekyll-Some-Pages-Cranky-Git %}) behind a couple of projects.

One of the things I'd considered at the time, and mentioned in [Projects Projects Projects]({% post_url 2018-11-02-Projects-Projects-Projects %}), is setting up a custom RSS feed for just the articles I wanted to submit at Dev.To. I plan on publishing a wide variety of articles here, and I know not all of them will be right for the community there, so I want to make sure I'm filtering out the rest. I tried just running my regular RSS feed to my profile there, but it left a lot of cruft on my dashboard in the *drafts*, and even if I deleted the drafts they would just show up again on the next refresh.

Which brings us to this bit - I've got a second RSS feed now with just the articles that I want to send over there.

In the front matter I have a `repost` variable like so:

![(side note: need to fix the highlighting/rendering of markdown code in posts&hellip;)](/img/2018-11-04-frontmatter.png '(side note: need to fix the highlighting/rendering of markdown code in posts&hellip;)'){class="pure-img"}
{% comment %}
{% include figure class="pure-img" image_path="/img/2018-11-04-frontmatter.png" alt="(side note: need to fix the highlighting/rendering of markdown code in posts&hellip;)" caption="(side note: need to fix the highlighting/rendering of markdown code in posts&hellip;)" %}
{% endcomment %}

Originally I was going to set up a "to-dev.to" tag, and go that way, but that didn't seem useful for the people who were visiting my site.

And there's now a `todev.to.xml` that filters through the posts for just those that I want to republish.

![DevTo XML](/img/2018-11-04-devtoxml.png){class="pure-img"}
{% comment %}
{% include figure class="pure-img" image_path="/img/2018-11-04-devtoxml.png" alt="DevTo XML" caption="" %}
{% endcomment %}

At my next opportunity, I'm going to try and pump it through the [Compress layout](https://github.com/penibelst/jekyll-compress-html) and see if that can get the size down without breaking anything. Though now that I think about it, I'd have to either adapt it to work with [Pretzel](https://github.com/Code52/pretzel) or do the Pretzel-to-Jekyll conversion first.

So there's the short version. I'm sure there's a more efficient way to do this, but I probably won't worry too much about it until I do the conversion to Jekyll. I don't plan on adding any more features before then.

(Hot damn! that makes 4 for 4 on my "[Almost NaNoWriMo]({% post_url 2018-11-01-Almost-NaNoWriMo %})"!)