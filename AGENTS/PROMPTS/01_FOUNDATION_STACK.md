# TASK 01 — DEFINIR STACK TÉCNICO DEL PROTOTIPO

## Objective
Select and document the technical stack for the browser-capable vertical slice of ANONYM_US_<2047>.

## Context
The project direction has been refined after pre-production review. The game is now conceived as a **stylized post-apocalyptic sandbox with procedural worlds generated from seeds**, inspired by advanced contemporary cities rather than tied to a single real-world city. The world may contain futuristic infrastructure that continues operating after civilization's collapse, including systems influenced by SYNAPSE.

The target visual direction is simple, distinctive and scalable rather than photorealistic: think low-poly / stylized 3D as a candidate, with strong atmosphere and systemic depth. The game also contains a fictional terminal/CRT layer representing the machine world.

The prototype must be fast to iterate, easy for AI agents to maintain, lightweight enough for the target development machine, and capable of scaling from a small generated test area to larger seeded worlds if the vertical slice succeeds.

The repository requires the terminal to remain a closed fictional simulation.

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
- The procedural seeded-world direction is now part of the design target.
- The vertical-slice scope remains small.
- Candidate stacks are evaluated against actual project needs, not generic popularity.

## Task
Evaluate at least these credible options against the project direction:

1. **Godot 4.x + GDScript** with stylized 3D as the primary representation.
2. **Phaser + TypeScript** with 2D/2.5D as the primary representation.
3. **Three.js + TypeScript** as a browser-first custom 3D stack.
4. **Canvas + TypeScript without a 3D engine** as a control/reference option.

Evaluate:

1. procedural seeded-world support;
2. stylized 3D / low-poly viability;
3. browser-capable execution;
4. exploration and world streaming/scaling potential;
5. terminal/CRT integration;
6. maintainability by AI agents;
7. state/scene/input management;
8. performance on the prototype target;
9. future desktop/mobile viability;
10. dependency and engine complexity;
11. testing/debugging workflow;
12. ability to scale only after the vertical slice is validated.

Choose one stack. Record the decision and rationale in `AGENTS/DECISIONS.md`, then update `TECH/ARCHITECTURE.md` with the concrete stack and implementation direction.

Do not implement gameplay in this task.

## Acceptance criteria
- One stack is selected.
- At least three credible options were compared.
- The procedural seeded-world requirement is explicitly considered.
- The decision is recorded in `AGENTS/DECISIONS.md`.
- `TECH/ARCHITECTURE.md` contains the selected stack and why it fits this project.
- No gameplay code was added.
- The decision does not contradict the master context.

## Tests / verification
- Verify the selected stack has an official documented local start/build/export path.
- Verify the selected stack can support the intended 3D/stylized direction without requiring a custom engine as the first milestone.
- Verify the architecture keeps game logic, world-generation rules and data independent from presentation where practical.
- Verify terminal behavior remains isolated from the host operating system.
- Verify browser export remains a supported target, while allowing native desktop development/testing when it is technically preferable.

## Documentation updates
Required: `AGENTS/DECISIONS.md`, `TECH/ARCHITECTURE.md`, `AGENTS/PROJECT_STATUS.md`.

## Handoff
Report the selected stack, rejected alternatives, reasons, documentation changed, verification performed, and the exact next implementation task.
