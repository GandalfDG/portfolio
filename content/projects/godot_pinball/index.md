---
title: Virtual Pinball System in Godot Engine
date: 2024-03-03T13:38:06-05:00
draft: false
summary: Developing a modern virtual pinball system in the open-source Godot engine
---

{{< lead >}}I got into virtual pinball with Zen's *Pinball FX3*, and I looked around for open systems that would allow me to design my own pinball games.{{< /lead >}}
The most active of the systems I saw was VPX, but I was dismayed when I installed it and starting messing around with it that it had a few major drawbacks from my perspective:

1. **It only works on Windows<a href="#asterisk">\*</a>**
    
    I daily-drive some flavor of Linux on all of my computers, and while I could dual-boot windows on my desktop it's not a very smooth experience

1. **The user interface looks like it hasn't been touched since the days of Windows 98**

    While some people on vpin forums are able to make really stunning tables in spite of this, I can't be the only one who's decided against making something because the interface doesn't look user-friendly

1. **It requires a lot of manual file management and tweaking to get tables up and running**

    Table files, ROMs and visual packs need to be put in their proper folders and sometimes visual basic scripts need editing in order to get tables to work properly.

With these and other issues in mind, I decided to start work on a new, modern virtual pinball system
in the open-source game engine, [Godot](https://godotengine.org).
While this project is still very much a work in progress, several reusable elements and utilities have
been developed to allow intuitive playfield design and testing in 3D. Through implementing these elements I've also laid the groundwork for extending the system with unique elements, composed of existing
physics behavior nodes. This has been a very interesting project to help me jump in at the deep end
of 3D game development, and I hope to continue working on it and pick up some new contributors who
can help add features, develop their own tables, and spread the word.

Eventually I'd like to build a community around this project including developers, designers and players.
Hopefully a system like this built in a modern game engine and focused on open-source will open the
door to a whole new crop of pinball designers who like me might have wanted something a bit more
user-friendly than VPX.

### Currently Implemented Elements:

- Flippers
- Pop Bumpers
- Spinners
- Drop Targets
- Rollovers
- Ball Guides
- Playfield Inserts

### Elements in Progress:
- Bezier curve-defined ramps
- Playfield cutout generator using *Constructive Solid Geometry* (CSG)

### Follow me on Mastodon for updates on the project

<iframe src="https://indieweb.social/@GandalfDG/111161833076030344/embed" class="mastodon-embed" style="max-width: 100%; border: 0" width="800" allowfullscreen="allowfullscreen"></iframe><script src="https://indieweb.social/embed.js" async="async"></script>

### Star the project on GitHub and contribute

{{< github repo="gandalfdg/pinhead" >}}

-----

<span id="asterisk"></span>*\* OK, technically I was able to get it working with WINE, but because it relies so heavily on Windows-specific APIs the performance wasn't satisfactory.*

