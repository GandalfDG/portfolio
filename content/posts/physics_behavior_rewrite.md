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
of this base node. Not only that, but *Godot* works much better with a "call down, signal up" flow. 