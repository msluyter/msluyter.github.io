---
title: "Hello World"
date: 2026-03-27
draft: false
tags: ["meta"]
summary: "A quick intro and a look at my first project — Neutron, a abstract strategy board game you can play in the browser."
---

Hi! I'm Mike Sluyter! It seems insane to start a blog in this day and age. What can I say that an AI doesn't already know? But I'm feeling punchy, so here we go...

## AI Stuff

Like a lot of folks, I've been caught off guard by how rapidly AI has progressed. Perhaps more on this later. For the moment, I'm trying to catch up.  

Quite a few years ago some friends and coworkers of mine ran across this small abstract game called [Neutron](https://en.wikipedia.org/wiki/Neutron_(board_game)), an abstract strategy board game invented by Robert A. Kraus in 1978. We decided to write a computer player for it. Like all of my other side projects, it didn't go very far, but iirc, I think I had a rough terminal interface in Perl -- yes! it was _that_ long ago! -- working.

I thought of this game again a year ago, and started writing something in Python. IIRC, it took several hours just to get basic piece moement mechanics fleshed out, and I didn't even get to a the computer player. 

Cut to a couple of weeks ago. I decided to retry creating a Neutron game with Claude. I had Claude read the rules, and implement the game in a single html page with p5.js. I've been amazed at how fast I've been able to move and how far I've gotten. It's been over 10 years since I've even looked at javascript. And for this project, I haven't even looked at the code. 

## Neutron

The game is played on a 5×5 grid. Each player has five soldiers on their home row, and a single neutral piece — the neutron — starts in the center. Pieces move as far as they can in a single direction, and stop when blocked by another piece or the edge of the board. The goal is to either a) move the Neutron to your home row or b) trap the Neutron so the other player can't move it. Players alternate, with each move consisting of moving the Neutron followed by moving a soldier. The first move of the game is an exception, and consists only of a soldier move.

"Bobail" is a variant where the neutron can only move one square, like the king on a chess board.

AFAICT, there's a forced win on a 5x5 board if you move first. I'm not sure about 7x7 or other variants. 

Give it a try: **[Play Neutron](https://msluyter.github.io/neutron/)**
