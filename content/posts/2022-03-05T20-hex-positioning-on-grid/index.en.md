---
author: Zageron
publishDate: 2022-03-05T20:13:35-08:00
title: "Hex Positioning on Grid"
slug: hex-positioning-on-grid
tags: 
- rust
- nodes
- hex
- tick
series: ["Isometric Game Project"]
draft: true
---

## Roll Your Own

> Reinventing the wheel _will_ teach you.

I've decided to use my own implementations of things for two reasons.

- I need to continue to learn and grow.
- Using prebuild libraries can cause choice paralyses.

While a forever controversial opinion, in this case I think it is valid.

---

## Starting with Entity Positioning

> Stand here. Okay, don't move.

I referenced the following repositories and articles for this section:

- [hex2d-rs](https://github.com/dpc/hex2d-rs)
- [RedBlobGames - Hexagons](https://www.redblobgames.com/grids/hexagons/)


---

## To ECS or not to ECS

> As usual, I get decision paralyses right at the start of any project.

It's always difficult to decide what to work on first,
and it's even more difficult to pick which library or tools to use.
Something I suffer from every single time is over-engineering right at the start.

The decision of whether to use an ECS or not is the first thing I've come across now.
While perusing the options, I came across this in the [hecs](https://github.com/Ralith/hecs#why-not-ecs) repository.

> **Why Not ECS?**
>
> ... If your game will have few types of entities, consider a simpler
> architecture such as storing each type of entity in a separate plain
> `Vec`. ...
>

This thankfully woke me up early, and I remembered the [**YAGNI**](https://en.wikipedia.org/wiki/You_aren%27t_gonna_need_it) principle. Until managing my entities becomes unwieldy, I will stick with managing my components myself.

---
