---
title: Teaching machines to beat me in chess
layout: default
---

# Teaching machines chess from first principles

I'm ~1800–1900 in Lichess Rapid, and like many serious hobbyists, I’ve thought a lot about how chess *works*. Tactics are explainable, but concepts like strategy and pressure are much harder to explain. I can feel it when my opponent is putting me in a suffocating position, but I would have a hard time teaching someone how to reproduce that feeling.

This is why I've always been fascinated with chess engines. The top engines are better than any human is, and I've always wondered:

> Is the engine good because it approximates strategy by grinding through tactical positions?
> Or do engines actually learn *strategy*?

There are broadly two ways to train a chess engine:

1. **Encode our existing human understanding.**  
   We can tell a computer how to value material. For example, a queen is worth more than a pawn.
   We can also provide heuristics that represent our opinions of best practices:
   * "Take the center"
   * "A knight on the rim is dim"
   * King safety
   * Important squares between opening, middle, endgame.
   This is how Deep Blue was trained to beat Kasparov and most of the engines I grew up with (OG Stockfish, Houdini) use this approach.

2. **Let the machine discover chess for itself.**  
   Just tell the machine the rules of the game and nothing else.
   Let the machine discover its own opinions from first principles.
   AlphaZero and Leela are trained in this way.

I wanted to understand the second approach — *not because it's better in practice* (Stockfish still beats AlphaZero at equal compute), but because it asks a more interesting question:


## Project goals
* 

## Memos
1. (Coming Soon) Board Representation
2. (Coming Soon) Convolutional Architecture
3. (Coming Soon) Policy and Value Heads
4. (Coming Soon) Monte Carlo Tree Search Integration

More content soon.