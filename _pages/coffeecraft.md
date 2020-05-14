---
title : CoffeeCraft
---

![CoffeeCraft Logo](/res/logo-coffeecraft.png){: class="pure-img"}

CoffeeCraft is a small, [HermitCraft](http://hermitcraft.com/)-like Minecraft server and podcast built with my sister and her husband. The three of us plan on posting weekly videos independently, a few live streams, and a few collaborative projects.

We're currently in what we're calling "Season 00", a private session where we get set up and start working out the rules for the server and how we're going to operate. I'm posting a live stream archive and all videos over on [my YouTube channel](https://www.youtube.com/channel/UCXafqhKHbkSUIrq0LAuu0tw). You can watch the live streams there, on [my Twitch stream](https://www.twitch.tv/anonjr_live), or on [my Mixer stream](https://mixer.com/AnonJr_Live). Twitch and Mixer should also have the last few live streams available for a bit.

You can get everything over at [CoffeeCraft.us](https://www.coffeecraft.us/).

## CoffeeCraft Posts
{% for post in site.tags["CoffeeCraft"] %}
 * [{{ post.title }}]({{ post.url }}) {% endfor %}
