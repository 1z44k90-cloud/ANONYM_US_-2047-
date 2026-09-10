# TASK 19 — PERSISTENCIA / SAVE STATE

## Objective
Implement or extend game save/load while keeping authoritative game state centralized.

## Required reading
- `AGENTS/MASTER_CONTEXT.md`
- `AGENTS/PROJECT_STATUS.md`
- `AGENTS/DECISIONS.md`
- `TECH/GAME_STATE.md`
- `TECH/ARCHITECTURE.md`
- GitHub issue

## Preconditions
The authoritative game-state model is defined and stable enough to persist.

## Task
Persist only the state required to resume the intended gameplay. Use a versioned save format when practical. Keep persistence independent from rendering/UI.

## Acceptance criteria
- Save and load preserve required state.
- Invalid or incompatible save data fails safely.
- Save format is documented.
- No duplicated authoritative gameplay state is introduced.
- Tests cover at least the critical serialization/deserialization path.

## Handoff
Report persisted fields, format/version, tests, migration considerations and known limitations.
