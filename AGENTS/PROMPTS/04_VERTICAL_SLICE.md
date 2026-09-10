# TASK 04 — INTEGRAR VERTICAL SLICE

## Objective
Integrate the validated foundation systems into the first complete playable loop.

## Required reading
- `AGENTS/MASTER_CONTEXT.md`
- `AGENTS/PROJECT_STATUS.md`
- `AGENTS/DECISIONS.md`
- `AGENTS/TASK_PROTOCOL.md`
- `TECH/ARCHITECTURE.md`
- `DESIGN/GAMEPLAY.md`
- `MISSIONS/001_CONTACT.md`

## Preconditions
Tasks 01–03 and their acceptance criteria are complete and merged into `main`.

## Task
Integrate the smallest loop:

`explore → interact → terminal → Julia contact → fictional infiltration puzzle → simulated payload → SYNAPSE detection/trace → escape → consequence`

Do not expand the world or implement late-game systems.

## Acceptance criteria
- The complete loop is playable from start to finish.
- Mission state survives the transitions between world, terminal and dialogue.
- SYNAPSE reaction is represented as game state, not real AI/network activity.
- The player can reach a clear success/failure/consequence state.
- No critical runtime errors occur.

## Tests
- Full manual playthrough.
- Regression test of player movement and terminal behavior.
- Verify mission state transitions.
- Verify save/load if persistence has already been introduced.

## Documentation updates
Update `AGENTS/PROJECT_STATUS.md` and relevant architecture/mission documentation.

## Handoff
Document the validated loop, known weaknesses, bugs and the next highest-value gameplay improvement.
