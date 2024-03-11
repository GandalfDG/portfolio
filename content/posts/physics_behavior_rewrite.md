---
title: 'PhysicsBehavior Rewrite'
summary: ''
tags:
    - Godot
    - Pinball
    - Godot Pinball Toolkit
    - GDScript
date: 2024-03-11T10:17:09-04:00
draft: true
---

{{<lead>}}
There are a lot of parts of a pinball machine that need to react in some way when the ball interacts with them. My *PhysicsBehavior*
node is the base class for all of these reactions.
{{</lead>}}

Since I'm learning [Godot](https://godotengine.org/) through working on my [*Godot Pinball Toolkit*](/projects/godot_pinball), I'm still trying to
figure out how the engine wants things to be architected. After taking some time away from the project, coming back I
found the existing code I had written for the *PhysicsBehavior* node to be overengineered and working against the tree of
nodes concept that *Godot* is built around.

## Existing Code

The original design of *PhysicsBehavior* was trying to automate connecting itself to signals from nodes higher up in the tree.
This turned out to be a bit of premature complication, especially once multiple layers of inheritance were built on top
of this base node. Not only that, but *Godot* works much better with a "call down, signal up" flow. I also added complexity by
adding warnings to display in the editor if the parent node wasn't emitting the proper signal, rather than having the parent
give context to the behavior node. This also caused odd behavior because nodes become ready from the most nested node on up,
so I was attempting to get data from higher up nodes before the _ready callback would happen and it just wasn't working reliably.
The main thing that it should've been able to detect is when that signal was added to the parent node to clear the warning, but
that didn't happen. I'm sure there's a way that it could've worked, but it will be an enhancement after more important parts of
the toolkit are implemented.

