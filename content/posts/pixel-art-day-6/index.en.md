---
author: Zageron
publishDate: 2022-06-09T11:50:52-07:00
title: "Pixel Art - Day 6 and blog"
slug: "pixel-art-day-6-and-blog"
tags: 
- pixel
- art
- game
- 2d
series:  ["Pixelized Art", "Isometric Game Project"]
draft: false
---

## Blog

I was busy for the last few days, but I did do stuff! 😨

### Reworking prototype foundation

- Switched from the 2D camera with the hex grid example.
- Implemented an orthographic projection and figured out movement and rotations.
(Rotations outside of an orthographic projection)
- Added some example items and a plane.
(Will remove this later and do a height variable hex debug grid.)
- Added a few debug fields to egui to allow quicker camera testing.


### Next steps

- Going to add rotations on the 45 degrees.
Rotation an orthographic hexagonal grid means that there are creative restriction options.
  - Since a hex grid has point up or point down orientations,
  a decision on how rotation will effect the grid must be made.
  Sprites will have 8 rendered directions,
  but will only be able to use 6 of them depending on which orientation the grid is in.

----


## Art (work in progress)

The Pixel Daily was "heroic",
 so I decided to create an isometric render of the hero sword pedestal.

![Hero Sword Reference](hero-sword-reference.jpg)

Here's my work in progress as of yesterday morning.

![Hero Sword Isometric WIP](hero-sword-iso-first-draft.png)

There is plenty wrong with it at first glance.

- It's very squashed.
- I'm going to stretch it to fill the entire 48x48 canvas.
- Stairs are missing
- It's not uniform.

Luckily / unluckily for me,
I somehow managed to not save at the start and restarted my computer.
Asesprite decided that this time it didn't count, and didn't do an emergency back-up for me.

No big deal, I'll start again! :D

That's all for this post, I might post again tonight with my progress.
