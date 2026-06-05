# Contributing to Tron Game

## Ideas for Extension
- Add AI opponent (single player mode)
- Add power-ups (speed boost, wall clear)
- Add mobile touch controls
- Add 3-4 player support on larger grid
- Add a leaderboard using localStorage

## Code Structure
All logic is in a single `index.html`. The main loop is `setInterval(tick, SPEED)`.
Key objects: `players[]`, `grid[][]`, `DIRS{}`.
