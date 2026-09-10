# TASK 02 — SHELL DEL JUEGO Y MOVIMIENTO DEL JUGADOR

## Objective
Create the smallest executable 2D/top-down foundation in which the player can move through a small fictional Tijuana area.

## Context
This task implements GitHub Issue #1 only after the technical stack decision in Task 01 has been accepted and documented.

The objective is to prove the foundation, not to build the complete game.

## Required reading
- `AGENTS/MASTER_CONTEXT.md`
- `AGENTS/PROJECT_STATUS.md`
- `AGENTS/DECISIONS.md`
- `AGENTS/TASK_PROTOCOL.md`
- `TECH/ARCHITECTURE.md`
- `DESIGN/GAMEPLAY.md`
- `DESIGN/VISUAL_STYLE.md`
- GitHub Issue #1

## Allowed files
Only the project shell, world/movement implementation and directly required configuration/assets. Update related documentation when behavior changes.

## Forbidden files
- Terminal engine implementation
- Full mission system
- Dialogue/Julia implementation
- Complex combat
- Advanced enemy AI
- Large open-world systems
- Real network/OS integrations

## Preconditions
- Task 01 has selected and documented the technical stack.
- Local project start/build commands are known.
- The project remains within vertical-slice scope.

## Task
Implement:
1. project shell;
2. small 2D/top-down test area inspired by the project's Tijuana setting;
3. controllable player;
4. keyboard movement;
5. camera/viewport behavior appropriate to the selected stack;
6. basic collision/bounds;
7. a minimal interaction-ready world structure without implementing the full interaction system.

Keep gameplay state separate from rendering.

## Acceptance criteria
- Project opens and runs locally.
- Player is visible.
- Player moves reliably with the intended keyboard controls.
- Camera/viewport behaves correctly.
- Player cannot leave the intended test area.
- No critical console/runtime errors occur during normal use.
- No terminal, real network or real OS functionality is introduced.

## Tests
- Run the documented install/start/build or equivalent commands.
- Perform a manual movement test.
- Verify collision/bounds.
- Check browser/runtime console for critical errors.

## Documentation updates
Update `AGENTS/PROJECT_STATUS.md` and any technical documentation affected by implementation details.

## Handoff
Report files changed, commands used, test results, controls, known limitations and the next recommended task.
