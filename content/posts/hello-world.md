---
title: "Hello World"
date: 2026-03-27
draft: false
tags: ["meta"]
summary: "A quick intro and a look at my first project — Neutron, a abstract strategy board game you can play in the browser."
---

Hi! I'm Mike Sluyter! I'll be detailing some of my adventures in coding here.

## Neutron

My first project is a browser-based implementation of [Neutron](https://en.wikipedia.org/wiki/Neutron_(board_game)), an abstract strategy board game invented by Robert A. Kraus in 1978.

The game is played on a 5×5 grid. Each player has five soldiers on their home row, and a single neutral piece — the neutron — starts in the center. On each turn, you first slide the neutron in any direction (it travels until it hits the edge or another piece), then slide one of your own soldiers. The goal is to get the neutron onto your home row.

It sounds simple, but there's real depth to it. The neutron is shared, so every move you make with it sets up your opponent's next turn. Positioning your soldiers to control the neutron's path is the key to winning.

The app includes:
- **Three AI difficulty levels** — Easy (random safe moves), Intermediate (minimax with alpha-beta pruning), and Advanced (iterative deepening with a time budget)
- **Drag-and-drop** and click-to-move input
- **A Bobail variant** where the neutron moves only one square at a time, like a chess king
- **5×5 and 7×7 board sizes**
- **Undo, resign, auto-restart**, and a game record pane

Give it a try: **[Play Neutron](https://msluyter.github.io/neutron/)**
