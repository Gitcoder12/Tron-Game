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

## Branch Activity & Development History

**Audit date:** 2026-11-18 · **Comparison base:** `main`

| Branch | Difference from `main` | Observed work / changed paths |
|---|---:|---|
| `docs/portfolio-operating-kit-2026-11-13` | 4 ahead / 3 behind | Activity log, agent guidance, company-fit notes, feature plan, README support docs and skills; README has both additions and removals |
| `docs/project-status-audit20261116` | Comparison unavailable | GitHub returned 404 for the comparison; recheck branch existence |

### Open pull requests observed during this audit

- [PR #2 — project status snapshot](https://github.com/Gitcoder12/Tron-Game/pull/2)
- [PR #1 — project roadmap, activity log and agent guides](https://github.com/Gitcoder12/Tron-Game/pull/1)

**Review note:** The portfolio branch changes README content as well as adding docs. Inspect its diff before merging. No branches have been merged or deleted by this documentation update.
