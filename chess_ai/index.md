---
title: Teaching machines to beat me in chess
layout: default
---

# Teaching machines chess from first principles

I'm ~1800–1900 in Lichess Rapid, and like many serious hobbyists, I’ve thought a lot about how chess *works*. Tactics are explainable, but concepts like strategy and pressure are much harder to explain. I can feel it when my opponent is putting me in a suffocating position, but I would have a hard time teaching someone how to reproduce that vibe.

This is why I've always been fascinated with chess engines. The top engines are better than any human is, and I've always wondered:

<div class="epigraph">
  <blockquote>
    <p><em>Is the engine good because it approximates strategy by grinding through tactical positions?</em></p>
    <p><em>Or do engines actually learn <strong>strategy</strong>?</em></p>
  </blockquote>
</div>

There are broadly two ways to train a chess engine:

1. **Encode our existing human understanding.**  
   We can provide heuristics that represent our opinions of best practices. This is how Deep Blue was trained to beat Kasparov and most of the engines I grew up with (OG Stockfish, Houdini) use this approach.
   <label for="mn-1" class="margin-toggle">⊕</label>
    <input type="checkbox" id="mn-1" class="margin-toggle"/>
    <span class="marginnote quote">
    In approach 1, some heuristics to consider:
    * We can assign values to material: Queen > Rook > Bishop / Knight > Pawn
    * "Take the center"
   * "A knight on the rim is dim"
   * King safety
   * Important squares between opening, middle, endgame.
   </span>

2. **Let the machine discover chess for itself.**  
   Just tell the machine the rules of the game and nothing else. The machine has to learn chess from first principles. AlphaZero and Leela are trained in this way.

It always felt mystical to me that a machine could see enough games and learn chess better than I've learned it through focused study, and I wanted to replicate that. The following is a summary of my findings as I built a **AlphaZero like neural network-based chess engine from scratch**.


## Project goals
* 

## Memos
1. (Coming Soon) Board Representation
2. (Coming Soon) Convolutional Architecture
3. (Coming Soon) Policy and Value Heads
4. (Coming Soon) Monte Carlo Tree Search Integration

More content soon.