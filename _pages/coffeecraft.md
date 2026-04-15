---
title : CoffeeCraft
description: "A summary of, and a rundown on all posts related to, the CoffeeCraft server and videos."
---

![CoffeeCraft Logo](/res/logo-coffeecraft.png){: class="pure-img"}

CoffeeCraft is a small, [HermitCraft](http://hermitcraft.com/)-like Minecraft server and podcast built with my sister, her husband, and a mutual friend. The four of us planned on posting weekly videos independently, a few live streams, and a few collaborative projects.

We're currently on hiatus. A live stream archive and other videos are over on [my YouTube channel](https://www.youtube.com/channel/UCXafqhKHbkSUIrq0LAuu0tw). You can watch the live streams there or on [my Twitch stream](https://www.twitch.tv/anonjr_live). (When I get back to streaming)

More information is over at [CoffeeCraft.us](https://www.coffeecraft.us/). We are using a couple custom resource packs I developed. More available [in these articles]({% link _pages/resource-packs.md %}).

## CoffeeCraft Posts
{% for post in site.tags["CoffeeCraft"] %}
 * [{{ post.title }}]({{ post.url }}) {% endfor %}
