---
title: 'Catching Up on Personal Projects'
summary: "I've been busy, but I finally feel like I'm back on track and ready to tackle projects again"
tags:
    - ''
date: 2025-04-01T18:57:34-04:00
draft: true
---

{{< lead >}}
The past few months have been a blur. My wife and I shot a TV show pilot, we moved in to our 
first home, we attended two weddings, one of which was in Disney World, and I'm sure I'm forgetting plenty of other
things that have kept me from "doing my own thing" for nearly three months.
{{< /lead >}}

Now that we're settling in at our new home, and the stressful move is behind
us I'm figuring out how to pick up the pieces of all the projects I've been
itching to work on while *truly* having no time for them.

## Getting Busy

My wife and I had planned on buying our first home sometime in the first half of 2025.
We had looked at some houses to get a lay of the land throughout 2024, but I knew that
I would be ready to pull the trigger in the new year. What I didn't expect was to find
something we really loved among the first few places we toured on the first weekend of 
January. I saw it on Saturday, I took Kiersten to see it on Sunday, and our offer was in
on Monday. And we didn't even have time to think because the seller was accepting no
later offers, and the open house was unusually crowded for such a miserable cold weekend
in New England.

I knew that it was sudden, that it would mean breaking our lease earlier than we had planned,
but I was already so exhausted from that whirlwind weekend of making our offer and then
giving a final number against one other remaining buyer, that I knew I wouldn't want
to do this all over again later on. Our offer was chosen, starting a whole month of
gathering up documentation for a mortgage application and running around like a headless
chicken until our closing at the end of the month.

Also during this month I directed and started editing the pilot episode of Kiersten's
kids TV show concept, *Lilypad Library* to be ready for her to pitch it at the Kidscreen
conference in mid-February. You can check out the pilot [here on youtube](https://www.youtube.com/@LilypadLibrary) 

![Lilypad Library Set](lilypad_set.jpg)

I'm very happy with what we were able to accomplish, but between the home
buying process, and singlehandedly trying to chroma key and cut video together, as well as
mixing and synchronizing audio for a twelve-minute episode I could feel my stress level
rising. (Shoutout to my past self for writing a post about [chroma keying in Blender](/posts/chroma_key_blender), I really
needed to refer back to this.)

## Moving out

February was split between packing up all of our posessions, finalizing the
edit of the *Lilypad Library* pilot, managing our relationship with our
landlord in an attempt to get out of our lease early, traveling to Long Island
for a wedding, and of course still working both of our full-time jobs. This was
where I truly ran out of spoons. I knew I had to get everything out of our old
place by the end of the month but as the piles of things dwindled it seemed harder
and harder to put them into boxes and load them into cars. We managed it in the end,
but I had really reached my breaking point after that final trip to our house.

At this point I was broken down and still didn't have time to do anything to refill
my cup. I was having to turn down board game nights, and even the thought of writing
a blog post was weighing on me. I didn't think I was ever going to feel back on track.

## Finding my motivation

I know I'm not the only person with an overflowing to-do list. These past months
have been so full of things that I *needed* to do that I really started to
wonder how I would ever recover from the lapse in project time. Now that enough stuff has been unpacked that I can generally return to my normal routines I've bee working hard to
*actively* get back to the projects I want to work on.

I'm keeping track of the things I have to do and trying to balance them with my ongoing
projects. Over a few weekends I got our main bathroom set up with shelves and a cabinet
from IKEA, which has given me confidence in drilling holes in our plaster walls. Alongside
that I spent time working on Kiersten's website to get it set up with a blog. I'm not 
much of a web developer, but I'm enjoying having a project to learn real HTML and CSS
frontend with. Making fun and responsive layouts is *no joke.* Here's a screenshot, but
go check it out live on [mskiersten.com](https://mskiersten.com/blog)

![blog list screenshot](blog_screenshot.png)

I'm still tinkering with it, but it's fun and functional enough to go live in my opinion.

## What's next?

Next on my list is getting back to reverse engineering my [Time Machine Pinball Machine](/posts/time_machine), I've been saving up ideas for updates
to the code ever since I got it. I'm excited to finally get back to some
low-level software on low-powered hardware, as a break from the higher-level
python I'm writing at work.

Here are my ideas in no particular order

<ul>
  <li>Balance starwarp either through scoring or by making spelling starwarp harder</li>
  <ul>
    <li>For example make only Einstein shots spell starwarp</li>
  </ul>
  <li>add a skill shot</li>
  <ul>
    <li>hit the top lane for the current decade for bonus points - maybe instantly qualify that decade, or at least spot two shots instead of one (though these are kinda the same thing)</li>
  </ul>
  <li>ball save</li>
  <ul>
    <li>use the extra ball light to indicate the ball save</li>
    <li>don't consume the kickback if used during ball save</li>
  </ul>
  <li>hold on to the ball at the vuk during the starwarp fanfare</li>
  <li>flash the lower left flasher before releasing a ball from the lock</li>
  <li>increase difficulty of starwarp and qualifying locks after each successful warp/multiball respectively</li>
  <li>unlimited kickback for a period at the start of multiball emulating a ball save</li>
  <li>Short ball save after kickback to give back ball if kickback failed by</li>
  <li>Play the song even if buy in is disabled</li>
  <li>Multiball restart if no jackpot</li>
  <ul>
    <li>Time limit to lock a ball</li>
    <li>If successful, kick out a ball and restart Multiball with 2 balls</li>
  </ul>
</ul>

I'm really excited to hone my assembly language skills by programming for 
the 6802 processor that runs the machine.

To wrap it up, even when you've been run ragged, you can be back on your
bullshit sooner than you think 👌