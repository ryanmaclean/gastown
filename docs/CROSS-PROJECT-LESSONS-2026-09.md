# Cross-project lessons — 2026-09

Gas Town is a valuable **control architecture** for the lower-bound agent-runtime research.

## What to compare

Gas Town uses Git/worktrees, Beads, SQLite queries, mailboxes, hooks, and persistent coordination state.

Compare that against:
- BOP filesystem state
- BOP + native filesystem history (HAMMER/LFS/FFS)
- smolFire/rump execution substrates

## Questions

- Which restart/handoff/ownership semantics truly require Git/Beads/SQLite?
- Which can collapse into filesystem-native identity/history?
- What is the memory/storage overhead per active agent?
- What coordination semantics should BOP explicitly keep because Gas Town proves they matter?

Do not merge Gas Town into BOP; use it as a feature/complexity baseline.

## Agent assignment

Copilot primary; `@codex` fallback.
