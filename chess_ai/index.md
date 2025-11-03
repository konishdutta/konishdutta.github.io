---
title: Teaching machines to beat me in chess
layout: default
---

# Teaching machines chess from first principles

I'm ~1800–1900 in Lichess Rapid, and like many serious hobbyists, I've spent a lot of time thinking about how chess *works*. Tactics are teachable, but to me, **strategy and pressure have always felt vibey**. I know it when I feel it, it's *hard to explain why*.

This is why I've always been fascinated with chess engines. The top engines are better than any human is, and I've always wondered:

<div class="epigraph">
  <blockquote>
    <p><em>Are engines strong because <b>they calculate tactics</b> well...</em></p>
    <p><em>... or because <b>they've learned strategy</b>?</em></p>
  </blockquote>
</div>

There are broadly two ways to train a chess engine:

1. **Teach the engine "good" chess.**  
   We provide heuristics that encode our opinions of what strong play looks like. This is how Deep Blue beat Kasparov, and how earlier versions of Stockfish and Houdini worked.
   <label for="mn-1" class="margin-toggle">⊕</label>
   <input type="checkbox" id="mn-1" class="margin-toggle"/>
   <span class="marginnote quote">
     In Approach 1, the engine doesn't *discover* strategy. We provide the engine our opinion of the best ways to evaluate chess and it applies that evaluation in its play.
   </span>

   Common heuristics we can encode:
   - Rewarding material (Queen > Rook > Bishop ≈ Knight > Pawn)
   - Control of the center (e.g. "A knight on the rim is dim.")
   - King safety
   - Different priorities across opening, middlegame, endgame

2. **Let the machine discover chess for itself.**  
   Just tell the machine the rules of the game and nothing else (no human guidance of what "good" chess is). The machine has to learn chess from first principles. AlphaZero and Leela are trained in this way.

It always felt mystical to me that a machine could see enough games and learn chess better than I've learned it through focused study, and I want to replicate that.

I'm building an **AlphaZero-style neural-network chess engine from scratch**.

This is the first in a series of engineering notes. The goal isn't to show just the result, but to speak to my reasoning in:

- Choosing a representation for the board and pieces
- Selecting a model
- Building a search and evaluation function
- Other decisions I don't know I have to make yet!

I intend the last note to be a look inside the layers of the final model, answering:

<div class="epigraph">
  <blockquote>
    <b>What do machines actually learn about chess when humans teach them nothing?</b>
  </blockquote>
</div>

## Project goals
* 

## Memos
1. (Coming Soon) Board Representation
2. (Coming Soon) Convolutional Architecture
3. (Coming Soon) Policy and Value Heads
4. (Coming Soon) Monte Carlo Tree Search Integration

More content soon.