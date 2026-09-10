# TASK 01 — DEFINIR STACK TÉCNICO DEL PROTOTIPO

## Objective
Select and document the technical stack for the browser-first vertical slice of ANONYM_US_<2047>.

## Context
The game is a hybrid 2D/top-down world plus terminal/CRT interface. The prototype must be fast to iterate, easy for AI agents to maintain, lightweight enough for the target development machine, and suitable for a future desktop/mobile path.

The repository already defines a modular architecture and requires the terminal to remain a closed fictional simulation.

## Required reading
- `AGENTS/MASTER_CONTEXT.md`
- `AGENTS/PROJECT_STATUS.md`
- `AGENTS/DECISIONS.md`
- `AGENTS/TASK_PROTOCOL.md`
- `TECH/ARCHITECTURE.md`
- GitHub Issue #2

## Allowed files
- `TECH/ARCHITECTURE.md`
- `AGENTS/DECISIONS.md`
- `AGENTS/PROJECT_STATUS.md`
- this prompt only if the acceptance criteria require clarification

## Forbidden files
- Gameplay implementation files
- Story/narrative files
- Terminal implementation
- Player movement implementation
- Unrelated project documentation

## Preconditions
- The project architecture has been reviewed.
- The vertical-slice scope remains small.
- Candidate stacks are evaluated against actual project needs, not generic popularity.

## Task
Evaluate the leading options (including Phaser + TypeScript, Godot and Canvas + TypeScript) against:

1. browser-first execution;
2. 2D/top-down development speed;
3. terminal/CRT integration;
4. maintainability by AI agents;
5. state/scene/input management;
6. performance on the prototype target;
7. future desktop/mobile viability;
8. dependency complexity;
9. testing/debugging workflow;
10. ability to scale only after the vertical slice is validated.

Choose one stack. Record the decision and rationale in `AGENTS/DECISIONS.md`, then update `TECH/ARCHITECTURE.md` with the concrete stack and implementation direction.

Do not implement gameplay in this task.

## Acceptance criteria
- One stack is selected.
- At least three credible options were compared.
- The decision is recorded in `AGENTS/DECISIONS.md`.
- `TECH/ARCHITECTURE.md` contains the selected stack and why it fits this project.
- No gameplay code was added.
- The decision does not contradict the master context.

## Tests / verification
- Verify the selected stack has a documented local start/build path.
- Verify the architecture remains platform-independent at the game-logic layer.
- Verify terminal behavior remains isolated from the host operating system.

## Documentation updates
Required: `AGENTS/DECISIONS.md`, `TECH/ARCHITECTURE.md`, `AGENTS/PROJECT_STATUS.md`.

## Handoff
Report the selected stack, rejected alternatives, reasons, documentation changed, verification performed, and the exact next implementation task.
