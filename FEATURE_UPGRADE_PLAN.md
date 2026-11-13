# Tron-Game — Feature Upgrade Plan

## Objective

A two-player browser game where light cycles move around a grid and lose when they hit a wall or a trail.

## P0 — correctness

- [ ] Add deterministic collision tests for wall hits, trail intersections, simultaneous collisions and edge wrapping rules.
- [ ] Test keyboard handling, focus behavior and restart logic across supported browsers.

## P1 — user experience

- [ ] Add configurable round restart and a clear pause/resume flow.
- [ ] Make canvas scaling and controls responsive for keyboard and touch without breaking the two-player mode.

## P2 — polish and performance

- [ ] Add optional local score history and game settings with documented browser storage behavior.
- [ ] Profile frame timing and ensure game logic remains deterministic at different refresh rates.

## Contribution work packages

1. Game-state and collision tests.
2. Input handling, accessibility and responsive canvas behavior.
3. Restart/pause/settings workflow.
4. Browser smoke testing and performance profiling.

## Definition of done

- [ ] Rules are documented and deterministic.
- [ ] Gameplay and collision edge cases are tested.
- [ ] README controls match actual key handling.
- [ ] At least one browser smoke test is recorded for UI changes.
