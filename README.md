# Tron Game

**A two-player light-cycle game that runs in a browser.**

[![License](https://img.shields.io/badge/license-see%20LICENSE-lightgrey)](LICENSE)

Tron Game is a small, dependency-free HTML5 Canvas game. Two players steer light cycles around a grid, leaving trails that become obstacles.

## Play

Open `index.html` in a modern browser. No installation or build step is required.

| Player | Controls |
|---|---|
| Player 1 | `W`, `A`, `S`, `D` |
| Player 2 | `↑`, `↓`, `←`, `→` |

## Rules

- Each cycle leaves a persistent trail.
- A cycle loses when it collides with a wall, boundary, or either trail.
- The last player still moving wins.

## Tech Stack

HTML · CSS · JavaScript · HTML5 Canvas

## Project Structure

```text
Tron-Game/
└── index.html
```

## License

See [LICENSE](LICENSE).

---

## Project handbook

- [Activity log](ACTIVITY_LOG.md) · [Feature upgrade plan](FEATURE_UPGRADE_PLAN.md)
- [Company and team fit](COMPANY_FIT.md) · [README explanation draft](README_ADDENDUM_DRAFT.md)
- [README quality checklist](README_QUALITY_CHECKLIST.md)
- [Contributing](CONTRIBUTING.md) · [Agent instructions](AGENTS.md) · [Agent skills](SKILLS.md)

## Understanding the project

### In plain language

A two-player browser game where light cycles move around a grid and lose when they hit a wall or a trail.

### Technical and research view

A dependency-free HTML5 Canvas game in a single-page application. Player one uses WASD and player two uses the arrow keys. Each cycle leaves a persistent collision trail. It is a small game project, not a multiplayer network service.

Document the update loop, input-state model, coordinate system, collision detection and restart lifecycle from the source code. Do not describe network multiplayer or features that are not implemented.

See [FEATURE_UPGRADE_PLAN.md](FEATURE_UPGRADE_PLAN.md), [ACTIVITY_LOG.md](ACTIVITY_LOG.md), [COMPANY_FIT.md](COMPANY_FIT.md) and [CONTRIBUTING.md](CONTRIBUTING.md) for technical depth and collaboration details.
