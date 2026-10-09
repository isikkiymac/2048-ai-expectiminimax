# 2048 AI with Expectiminimax

An intelligent agent that plays the 2048 game using expectiminimax search with alpha-beta pruning and tuned heuristics.

## Overview
Built as part of Columbia University's Artificial Intelligence course (COMS 4701). The agent models 2048 as a two-player game (player moves tiles, computer spawns tiles) and uses expectiminimax with alpha-beta pruning to make decisions within a strict 0.2s/move time limit.

## Tech Stack
- **Language:** Python
- **Algorithm:** Expectiminimax with alpha-beta pruning
- **Game Framework:** Provided Grid/GameManager skeleton (read-only)

## Key Features
- **Expectiminimax algorithm** — handles the probabilistic nature of tile spawning (90% chance of 2, 10% of 4)
- **Alpha-beta pruning** — significantly reduces search space
- **Heuristic functions:**
  - Available cell count
  - Monotonicity
  - Smoothness
  - Merge potential
  - Weighted combination for optimal play
- **Time-bounded search** — ensures move returns within 0.2s

## Results
- **Consistently achieves 2048+ tiles**
- **Under 0.2s per turn** — meets strict time constraint
- Outperforms random baseline by orders of magnitude

## What I Learned
- Adversarial search in stochastic games
- Expectiminimax vs minimax
- Alpha-beta pruning implementation
- Heuristic design and weight tuning
- Time-constrained search under hard deadlines

## Note
This project was completed for a course. Source code is available upon request due to course policy restrictions. I'm happy to discuss the search algorithm, pruning strategy, and heuristic tuning in an interview.
