---
title: AI and my Council of LLMs
description: There's been a lot of chatter about 'AI' use and LLMs and I wanted to stake out what I am and am not doing, as well as some opinions on the current discussions.
date: 2026-08-21 14:00
tags:
    - meta
    - programming
    - projects
repost: ""
---

Wow. There's been a lot going on about &ldquo;AI&rdquo; and it's use in the creative process. Or at least in content generation. And coding. And checking coding and content. And anything else anyone can find a way to be happy or sad or mad (whatever looks like it will get those clicks) about &ldquo;AI&rdquo;.
<!--more-->

## First Things First

Before I delve into the subject, and what I am and am not using, I want to make sure we're all on the same page with the terms going around. The same kind of loose language that made 5G and other technical terms nearly impossible to discuss are currently abusing the term &ldquo;AI&rdquo;. Artificial Intelligence, AI, is a very broad umbrella term that covers a lot of different things.

Sometimes when people are talking about AI they're talking about some sort of machine learning. Sometimes it's just a particular type of algorithm. Here lately it's likely either an LLM (Large Language Model) like ChatGPT, Copilot, or Claude; or a similar generative model like DALL-E and Nano Banana for images, or Suno and Lyria for music. All the while forgetting that technically spelling and grammar checkers are AI, as is your typical search engine. So unless the anti-AI folks are avoiding Google, Bing, Duck Duck Go, etc. to search for stuff, they're still technically using AI too.

Usually what I see people talking about now is the various generative models, be it LLMs for text or the similar music and image programs. Sometimes, because the term AI is being used in the discussion, there's a mistaken subtext of reasoning &mdash; close to, if not thinking of it as, AGI (Artificial General Intelligence). I'll try to be clear about what I'm referring to as we move forward.

## Playing With LLMs

In the [2024 Listener Hangout Show][1] I had mentioned that I hadn't really done much with LLMs beyond some research assistance and answering some interesting questions that came up in a D&D campaign (who knew that a barrel with all that coinage could still be floated through the underwater tunnel so long as it was properly sealed). Since then, I've been playing around with a few different LLMs a little more.

Google's Gemini has been getting more use whether I wanted to or not simply because Google is replacing its regular assistant in Android with Gemini. For some things, I haven't noticed that big a difference &mdash; asking random questions like the cast of the show I'm watching, or similar search stuff. For some things, it's definitely been a step back. Asking Gemini to pause audio while I'm driving used to be simple: shout "Hey Google, pause playback." and the podcast/music is paused. Now? Because of the audio ducking it "helpfully" tells me that there's no audio to pause. But the specifics of Gemini on Android phones are a different discussion. As a general purpose LLM it's been pretty good about some things, and less helpful about others. I'll get into specifics shortly.

I've been using ChatGPT a little longer than Gemini, and mostly at the recommendation from my middle sister, who's taken to affectionately calling him "Geeps" (soft "G" like Jiff, not the hard "G" like GIF 😉). Like Gemini, it's been pretty good about some things, less helpful about others. Depending on the task the better answer is often ChatGPT being slightly better than Gemini, or occasionally the other way around. I'm still working off the free plan, and will continue to do so until it makes financial sense to do otherwise.

Honorable mention goes to Microsoft's Copilot. Since I have an Office 365 subscription, I figured I'd give Copilot a little more of a workout. I used it for some of the same tasks I'd used the other two, and the performance was &hellip; uneven. Helpful often enough to not discard outright, but often dropping context or mixing things up that were understood earlier in the chat. Of the three, I would not recommend Copilot as a sole use solution. Even for programming, which is where I had expected it to excel.

## Council of LLMs

After spending some time bouncing between the three and getting a feel for where they can and can't help, I decided that instead of settling on just one LLM I'd make an LLM Council.

{% include figure image_path="/assets/img/2026-08-21_LLM_Council.png" alt="Council of LLMs" caption="Council of LLMs. Ironically enough, made by Copilot." %}

Since it was always a tossup between which was better, and there's value in using more than one model, I now have a tab group pinned and dubbed my &ldquo;LLM Council&rdquo;. I sometimes still ask just one of them to accomplish a task &mdash; like I recently used ChatGPT to troubleshoot some issues with mom's dishwasher, or I just used Gemini to troubleshoot an Android related issue on my phone &mdash; but more often I'm giving each of them the same prompt, comparing the results, and synthesizing what I want out of them.

Sometimes it doesn't quite work out. I've got a refurbished M1 MacBook Air that I was using occasionally when traveling to visit family or go to doctor's appointments. When I got it in 2024 I tried to set it up for some of the web work and programming I do. VS Code installed fine, as did most other things that had a Mac option, but getting Ruby and Jekyll installed was &hellip; an adventure. I ended up leaving the dev side of things in a slightly broken state as I could do everything I really needed to outside of a local build to preview work before publishing. Recently I've been trying to provide some love to the various neglected web projects (including this website). For a variety of reasons I've been on my laptop more, and so I needed to get Ruby and Jekyll fixed and working. In addition, I wanted to start automating more with PowerShell, so I wanted that working too. I initially tried the Council route, but all three started in very different places, and were looking to very different trajectories, so I decided to just get it working via ChatGPT and give the others an update on my current dev environment. That way any future questions would have the correct context for what I have running.

Most of the time though, despite the differences, it's worth getting all three involved. Even if Copilot is only rarely helpful. I've been trying to learn PowerShell in the context of an automation script I want to develop (more on that soon), and they've all been good on the teaching side. More importantly, they've each brought up things that the other two neglected. Often times though it still takes a person with at least the first principles understanding of programming to put it all together into some proper code.

{% include figure image_path="/assets/img/2026-08-21_Vibe_Coding.png" alt="Old Man Vibe Coding" caption="How I feel getting an LLM assist in programming. I selected the image generated by ChatGPT this time." %}

## What I Use

Inspired by a recent [Rands post][2] I want to stake out what I am and am not using these various tools for.

If you want to get technical, the spell checkers, grammar checkers, and various HTML/Markdown linters are all &ldquo;AI Tools&rdquo;. For posts like this and the first draft of static pages I've got a couple VS Code extensions being all sorts of annoying about my spelling and grammar. Sometimes I fix it. Sometimes I don't care that I accidentally used the British spelling instead of the American spelling. But for the most part, I try to get basic proofing on text and syntax done (even if a few typos still manage to escape).

For static pages I do run the copy through the Council for copy editing and to keep the readability metrics as close to where I want them as possible. These days the help is even more needed. In the [last post][3] I tried to address the rough overview of my &ldquo;survive cancer&rdquo; side-quest. One of these days I may even fill out a fuller and proper telling of that journey. Relevant to this discussion, the cancer treatment process has left me with some [Cancer Associated Cognitive Impairment][4] (at least that was the term used in the Duke [MAAT][5] sessions, Wikipedia lists it differently). I have days where there's still some real brain fog, where there's problems recalling a term, name, or definition, and days where there's genuine value in dropping all the thought fragments bouncing about and having them collated and presented back to me. In the end, they're still my thoughts, still me. It's like [rubber ducky debugging][6] for thoughts, but where the duck talks back.

I still use the council for some preliminary research, though I almost always use it as a starting point for further research. It's been helpful for trying to set up a set of bow length bench marks (marks on the bench to indicate things like if a bow is for a 4/4 or 3/4 violin, the origin for the term), mathing out how many hands high the Great Dane puppy is (he's currently 7.1 hands at 6 months old) because my youngest sister is a horse lover and I thought the reference would make her smile, and parsing stuff like DMARC reports and technical logs. I've found it well worthwhile to double-check things, as sometimes there's some bias shown in the sources used (as I've found in Bible research), and sometimes rules/context gets lost somewhere in the middle of something (looking at you Copilot) and the quick NPC you need generated for a game turns out to be a few skill points short or despite my correction the LLM keeps getting the max crew for a D&D 3.5e Carrack wrong.

{% include figure image_path="/assets/img/2026-06-09_ChewiePlaying.jpg" alt="Chewie the Great Dane playing" caption="Such a playful Great Dane. He's named Chewie, partly because the brindle pattern is reminiscent of Chewbacca and partly because he grumbles at you like a Wookiee." %}

I've also been using generative models for creating images, like the two before the photo of Chewie. Of any use I've mentioned so far, and any use I'll get to, this is probably the one that stirs up the most people. I have modest graphics design skills, and I'll use those when I can. When I can't do it myself I'll do the best I can with the tools available. I was originally going to opine on this a little more, but this is getting long enough for what it is, so I'll save that for another day.

Fun side note: I ran the same prompt through all three LLMs when I generated the images above. Copilot was the only one to put the clear &ldquo;Made with AI&rdquo; label in the upper-right corner. As I understand it, Gemini does something to the image that makes it identifiable as being generated. ChatGPT is the only one I'm not sure of, though I suspect that like Gemini there's something embedded that can be used to tell where it came from.

Lastly, I do use the Council as a coding assistant. I try to write what I can as best I can, fix it if I can with some quick searches, but for the more troublesome stuff &mdash; like odd edge cases in the way Jekyll processes things &mdash; I end up running it through an agent or three. And like I mentioned earlier, I'm using the Council to learn new languages. Last time I did any serious automation work was for the Hospital I worked at, and it was all VBScript. I could write the publication automation I want to do in VBScript, but why? Because I know it? It's past time I learned PowerShell and I don't have access to people I can learn from. This has been the next best thing.

I don't think it's for everyone though. There's real value in understanding programming from a first-principles mindset that allows you to look at what's generated in a new language, examine the explanation, and ask the right kind of clarifying questions to determine if the code is actually good or not. (&ldquo;AI Slop&rdquo; is thrown around to carelessly to be useful, I've avoided the term so far and will stubbornly persist in doing so for the remainder of this post.)

## What I write

All posts, and the scripts (where there are any) for projects like Games Revisited, Bible By Example, etc., are all me. The thoughts and initial text for static pages is all me, and the final selection is proofed and chosen by me &mdash; nothing is random blind copy/paste from a generic "write me a&hellip;" prompt.

The plan and direction for coding projects is me. The 14 years I wrote training software for the Hospital was as a sole developer. With the LLM Council it's odd being a project manager for 3 interns with some odd quirks.

## Conclusion

At some point I'll put together an abbreviated version of this so it will appear in the appropriate place when I get everything cross-posted to Substack. And I'll add something to the footer, so there's a reference available to those who just want to know.

I don't know if this will be useful or the source of the frustrating kind of &ldquo;feedback&rdquo;, time will tell.

[1]: https://youtu.be/S0Kpe77UEJY
[2]: https://randsinrepose.com/archives/how-grumbles-helps/
[3]: {% post_url 2025-12-02-Alive-and-Well-Mostly %}
[4]: https://en.wikipedia.org/wiki/Post-chemotherapy_cognitive_impairment
[5]: https://academic.oup.com/book/30618?login=false
[6]: https://rubberduckdebugging.com/

<!--

Starting prompt for LLM Council Image:

    I'm writing up a blog post about my "LLM Council" and how I use it. To riff on the way some people treat LLM content and the companies that are behind them, I'd like a meme-style image of three shadowy figures sitting behind a structure you'd normally see a pannel of judges or something like that. In the center is a faceless guy in a suit with a name tag labled "ChatGPT", on his left is a similarly attired guy with the name tag "Copilot", and on his right is a similarly attired guy with the name tag "Gemini"

Starting prompt for Vibe Coding Image:

    I'm looking for an image in the style of a newspaper editorial cartoon showing an old, bald, bearded man in country overalls and boots rocking in a rocking char typing on a laptop saying "Is this vibe coding?"

-->
