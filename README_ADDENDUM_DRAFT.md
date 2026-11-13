# Tron-Game — README Explanation Draft

## In plain language

A two-player browser game where light cycles move around a grid and lose when they hit a wall or a trail.

## How to play

Player one steers with W, A, S and D. Player two steers with the arrow keys. Avoid the arena walls and every trail. The last cycle that has not collided wins.

## Technical explanation

A dependency-free HTML5 Canvas game in a single-page application. Player one uses WASD and player two uses the arrow keys. Each cycle leaves a persistent collision trail. It is a small game project, not a multiplayer network service.

Document the update loop, input-state model, coordinate system, collision detection and restart lifecycle from the source code. Do not describe network multiplayer or features that are not implemented.

## Validation and contribution

Use FEATURE_UPGRADE_PLAN.md for tasks, CONTRIBUTING.md for workflow and ACTIVITY_LOG.md for test evidence.
