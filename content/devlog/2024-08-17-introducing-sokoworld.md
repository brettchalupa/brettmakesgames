+++
title = "Introducing SokoWorld: Early Access Release"
description = "Sharing initial details of the project and what's next"
date = "2024-08-17"
tags = ["SokoWorld", "Rust", "Macroquad"]
+++

![pixel art dog next to a box SokoWorld Classic box pushing puzzler](/SokoWorld-Logo.png)

A week ago I started working on a puzzle game called **SokoWorld**. It's an implementation of Sokoban, the classic box pushing puzzler that's deceptively simple and quite addictive. Today I've released **v0.1.0** of the game, an initial functional version with 20 levels. It's playable. But not very polished. And I've got a lot of ideas for where I want to take it. But it's a solid start!

My goal with the project is to ship a finished, polished puzzle game that's free and open source.

[Go play the game in your browser!](https://brettchalupa.itch.io/sokoworld)

## Inspiration

The inspiration for **SokoWorld** came from [a video by Lazy Devs Academy about great game projects for beginners](https://youtu.be/4TxIS3Zi_RQ?t=1591), where Sokoban is mentioned. Lazy Devs Academy is primarily a channel focused on making games with Pico-8, and I really enjoy all of their videos. I searched around to find out what Sokoban games exist on Pico-8 and found the wonderful [Sokobird by shyfu](https://shyfu.itch.io/sokobird), which instantly clicked in my head and got the gears churning.

The next day I dove into starting SokoWorld, as well as playing a bunch of levels and researching the game a little bit more deeply.

The motivating idea and aspiration for the project is: **what if there was Mario Maker but for Sokoban**?

We'll see if I can achieve that and if there's a community interested in it. But for now, I'm starting small and going to work out in the open.

## Why a Sokoban Client

![sokoworld puzzle screenshot](/SokoWorld-Screenshot-1.png)

A Sokoban client may seem a little bit basic... but that's actually just what I'm looking for! Something I can start, finish, add my own unique touch to, and expand upon. It's low stakes. I'm building the game using the Rust programming language with the Macroquad game library. I'm learning a lot, and taking on an interesting but small project is a perfect fit.

Because the rules of Sokoban are so simple, it means I can focus on a few aspects that are important to me:

- Piecing together and shipping a game in Rust
- Designing levels to grow at the skill
- Becoming a better pixel artist (right now I'm using a lot of freely avaialble sprites)
- How to polish a game
- Build tooling for quickly creating and testing levels

A lot of these skills will help with future projects.

## Why Rust

I'm quite interested in working with a lower level language than Ruby and TypeScript, the two languages I've primarily used throughout the past 10 years of my life. Rust's ecosystem, tooling, and approach to safety are all really appealing to me. I want to grow as a programmer, and I think Rust is a good way to do that. Combine that with game programming, and I'm hoping it leads to personal improvement, enjoyment, and interesting projects.

## Why Macroquad

There's a pretty good variety of different game programming libraries for Rust. I went with Macroquad because of the following reasons:

1. It's actively maintained
2. It's got a simple API that I could learn quickly
3. It doesn't force you to use a specific architecture, like Entity Component System (ECS)
4. It's supports building games for the web (WASM)

I've enjoyed getting to know the library and the community. It's been a good fit for the project so far.

## Open Source

Speaking of the code, the game is totally open source. The code is public domain. [You can view it on GitHub.](https://github.com/brettchalupa/sokoworld)

I'm hoping that by making it open source, other folks can learn from it and contribute to it if interested. Whether it's levels, features, or fixes, all are welcome. I'd love it if SokoWorld becomes a long-standing, feature-filled Sokoban client for years to come. The game being open source and free seems like a great way to help set that up to happen.

## Highlights

My favorite parts of working on the game so far have been:

- Designing levels and having fun doing it. The pipeline is quite nice—all I have to do is edit a text file and press a key to reload it. Testing the levels I design is quick, and often one level leads to designing another slightly modified.
- Getting to learn Rust and the ecosystem. The language nad tooling are quite great for what I look for in a language. I'm thinking about memory and performance more than past game projects, and that's been rewarding and interesting.

## Challenges

My attempt at pixel art (the Retro tileset) doesn't look so great! I'd like to take some time to study and practice pixel art.

Also, sometimes designing levels can be difficult. I have to be in the right headspace to experiment and try things.

## What's Next

I've got a lot of ideas planned for the immediate future and longer term. Hopefully this project doesn't go much longer than a few months, but I'm here for the ride wherever it takes me. I'd like to at least get it to v1.0, see how it is received, and distriute it far and wide.

Here's what's on my mind for what's up next:

- Save levels beaten and steps and pushes
- Desktop builds since right now it's just on the web
- Add a bunch more levels
- Rewind support
- More polish and improve user interface
- Resolution independent UI (currently set to 1280x720 and scales)

Some bigger ideas I have (but we'll see if I get to them):

- Release on iOS & Android
- Ability to play custom level packs from a folder on computer
- Built-in level editor
- Server for publishing and listing out level packs (similar to Mario Maker)
