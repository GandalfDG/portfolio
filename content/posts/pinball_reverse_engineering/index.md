---
title: 'Reverse Engineering My Pinball Machine'
summary: "I bought a pinball machine. A Motorola 6808 runs the show, so let's reverse engineer the ROM and maybe add some new features!"
tags:
    - Electronics
    - Programming
    - Pinball
date: 2024-07-11T14:18:12Z
draft: true
---

{{< lead >}}
I bought a pinball machine from the 80s, namely *Time Machine* by Data East. A Motorola 6808 
processor runs the game, so I wanted to see what I could learn from reverse engineering the ROM.
{{< /lead >}}

This will be my first foray into binary reverse engineering. I will be using Ghidra to help with
the disassembly process and hopefully to make my own modifications to the game. For instance, this
game doesn't have a timed ball save which would make the game a lot more friendly to new players.

## Memory Layout
The game's code is split across two ROM chips which reside at the top of the 6800's memory space.
The CMOS RAM chip is at the bottom of the address space, and the Peripheral Interface Adapter (PIA)
chips are addressable in between the RAM and ROM.

## Interrupt Vectors

## Peripherals