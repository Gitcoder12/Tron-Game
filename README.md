# Tron Game

Two-player Tron light-cycle game in a single HTML file. No dependencies, no install.

## Play

Open `index.html` in any browser.

| Player | Controls |
|--------|----------|
| P1 (Cyan) | `W A S D` |
| P2 (Red) | `↑ ↓ ← →` |

## Rules

Move your light cycle across the grid. Your trail is a wall. Hit any wall — yours, your opponent's, or the boundary — and you lose. Last cycle alive wins.

## Stack

Vanilla HTML5 Canvas + JavaScript. Zero dependencies.

## Author

Dharavath Satvik — [github.com/Gitcoder12](https://github.com/Gitcoder12)


---

## AI-maintained project notes (secondary — 2026-11-13)

This section supplements the maintainer-authored README above. The original text has been restored verbatim from Git-history baseline `f72c8b7fdcde5ba96083de127731d04f03f93db1`; this addendum does not replace or certify the original claims.

- The current source tree, runtime data and tests are the implementation source of truth. Roadmap items, draft PRs and AI-generated descriptions are not shipped features by themselves.
- Preserve real and maintainer-provided data. Never silently substitute generated or placeholder data. Clearly label and isolate synthetic fixtures.
- Mark unverified sources, identifiers, metrics, benchmark results and external claims as unknown/unverified rather than guessing.
- Verify setup, execution, tests and public claims against the exact current commit before using this repository in a job, research or academic application.
- See [MODEL_AUDIT_ROUTER.md](MODEL_AUDIT_ROUTER.md) for independent model review instructions and the merge gate.

---

## Engineering Audit & Handover — 2026-11-17

**Reviewed commit:** `2dd8ec3c356c538a53e8ace52515d37a8f665cab` (`main`).

### Confirmed findings
- The reviewed implementation is a single-file browser game (`index.html`) with no automated test suite in the reviewed tree.
- The README accurately describes a local two-player game and keyboard controls; collision, restart, and simultaneous-input behavior have not been independently verified in this audit.

### Next actions
1. Add a small deterministic test harness for movement, wall/trail collision, and winner selection.
2. Verify keyboard behavior and responsive layout across desktop browsers.
3. Document any known limitations such as touch/mobile controls if they are not supported.

**Verification status:** source-tree inspection only; no browser play-through or automated test was run.

---

## Examples Used
- Two light cycles competing in a grid arena
- Detecting a collision with a trail or boundary
- Determining the last surviving player


---

## Comparison with Existing Open-Source Projects

Tron Game is a small, browser-based two-player light-cycle game implemented in a single HTML file. The following projects are useful comparisons for implementation approach and game-development infrastructure rather than exact feature competitors.

| Project | Established focus | Relationship to Tron Game |
|---|---|---|
| [Phaser](https://github.com/phaserjs/phaser) | Full-featured 2D HTML5 game framework | Provides scenes, input, physics and asset tooling; this project deliberately avoids a framework for a compact single-file game. |
| [PixiJS](https://github.com/pixijs/pixijs) | High-performance 2D WebGL renderer | A rendering library rather than a ready-made Tron game; the current project uses the browser Canvas API directly. |
| [raylib](https://github.com/raysan5/raylib) | Simple cross-platform game-development library | A broader native game-development toolkit; this project targets immediate browser play with no installation. |

### Where Tron Game is different
- **Zero-install browser play:** the documented game opens directly from index.html without a build step or dependency installation.
- **Two-player local controls:** both players share one keyboard and one grid arena, keeping the core game loop easy to understand.
- **Minimal implementation:** Canvas and vanilla JavaScript keep the project small and approachable for studying collision and movement logic.

### Where established projects are stronger
Phaser, PixiJS and raylib provide far richer rendering, input, asset, audio and cross-platform facilities. Tron Game does not claim to compete with those frameworks; its value is a small, inspectable example of a classic local multiplayer game.

### Evidence and limitations
This comparison is based on the README's single-file implementation description. Feature parity, frame-rate behavior, browser compatibility, accessibility and mobile/touch controls have not been benchmarked here. Add deterministic tests for movement, collision, simultaneous inputs and winner selection before making reliability claims.
