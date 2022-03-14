---
author: Zageron
publishDate: 2022-03-21T08:00:00-08:00
title: "Entity and Graph Association"
slug: "entity-graph-association"
tags:
- rust
- graph
- entities
series: ["Isometric Game Project"]
draft: true
---

## Outline and Goal

Games usually need a clear way of representing entities, their data, their position in the world,
and ways they might interact with one another. For this game I'll be using a simplified variation of ESC,
where I store my own entities in my own hash tables.

For positioning, I need to restrict my design temporarily to simplify the implementation.
Eventually I want to have fluid movement between nodes,
but for now I think that having absolute and instantaneous positioning will be sufficient.
So for now position will be controlled directly by the associated node / hex.

For movement, I'll stick to `WASD` for now. Six direction means that the control isn't uniform.
Depending on the orientation of the graph, that means:

> `WD, D, SD, SA, A, WA`
> or
> `W, WD, SD, S, SA, WA`

---

## The Entity

---

## Storing the Entity

---

## Associating an Entity with a Node

---

## Granting Position to an Entity

---

## Moving an Entity "Around the Graph"
