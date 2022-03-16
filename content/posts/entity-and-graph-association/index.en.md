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

## Clean-up from last time

First things first, I was not happy with the module hierarchy in gamecore.
So I switched up the file structure and updated the way imports and exports were done.

### Gamecore

<!-- omit in toc -->
#### Before

```txt
src/
├── graph.rs
├── hex.rs
└── lib.rs
```

`lib.rs`

```rust
pub mod graph;
pub mod hex;
```

<!-- omit in toc -->
#### After

```txt
src/
├── types/
│   ├── graph.rs
│   ├── hex.rs
│   └── mod.rs
└── lib.rs
```

`mod.rs`

```rust
mod entity;
mod graph;
mod hex;

pub use entity::*;
pub use graph::*;
pub use hex::*;
```

`lib.rs`

```rust
pub mod types;
```

### Render

<!-- omit in toc -->
#### Before

`render/main.rs`

```rust
use gamecore::{graph::Graph, hex::Hex};
```

<!-- omit in toc -->
#### After

`render/main.rs`

```rust
use gamecore::types::{Graph, Hex};
```

> Much better!

---

## The Entity

- Add the Entity structure.

---

## Storing the Entity

---

## Associating an Entity with a Node

---

## Granting Position to an Entity

---

## Moving an Entity "Around the Graph"
