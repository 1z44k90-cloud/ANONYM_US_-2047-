# DECISIONS — ANONYM_US_<2047>

This is the architectural and process decision log. Decisions recorded here are authoritative until explicitly superseded.

## DEC-001 — Agent development workflow
- Status: ACTIVE
- Decision: AI agents must use a controlled loop: READ → PLAN → IMPLEMENT → TEST → REVIEW → DOCUMENT → UPDATE STATUS → HANDOFF.
- Reason: prevent duplicated work, contradictory changes and unfinished handoffs.
- Consequence: an agent is not finished when code merely exists; it must leave a tested, documented and understandable state.

## DEC-002 — `main` is the stable branch
- Status: ACTIVE
- Decision: `main` represents the latest approved/integrated project state. Agents must not use `main` as their normal working branch.
- Workflow: task `.md` → feature branch → implementation/tests/review → pull request → merge to `main`.
- Reason: preserve a reliable baseline and make changes auditable.
- Consequence: experimental or incomplete work stays outside `main`.

## DEC-003 — Documentation is part of the product source of truth
- Status: ACTIVE
- Decision: project intent, architecture, process, phase status and important decisions must live in version-controlled repository documentation.
- Reason: future agents need durable context that does not depend on conversation history.
- Consequence: undocumented architectural changes are considered incomplete.

## DEC-004 — One coherent system per agent task
- Status: ACTIVE
- Decision: an agent owns one coherent area per task and communicates with other systems through explicit interfaces/state.
- Reason: reduce hidden coupling and conflicting edits.
- Consequence: an agent must not redesign another system silently.

## DEC-005 — Architectural conflict protocol
- Status: ACTIVE
- Decision: when an assigned task conflicts with an existing decision, the agent must stop before expanding the conflicting implementation, document the conflict and propose a resolution.
- Reason: prevent silent architectural drift.
- Consequence: the master context and decision log remain internally consistent.

## DEC-006 — Terminal/network safety boundary
- Status: ACTIVE
- Decision: all terminal, credentials, malware, exploits and network behavior are fictional game mechanics isolated from the host operating system.
- Reason: preserve the game's design while preventing real-world operational functionality.
- Consequence: no real unauthorized-access or malware functionality belongs in the game code.

## DEC-007 — User authorization for project-governance decisions
- Status: ACTIVE
- Decision: the assistant may make reasonable, reversible decisions that improve the completion and internal consistency of the GitHub documentation/governance system without requesting separate approval for every minor documentation choice.
- Scope: documentation structure, prompt organization, status-board conventions, agent workflow wording, review/handoff templates and similar project-governance details.
- Constraint: this authority does not permit silently changing core game canon, major technical architecture, scope, story outcomes or other substantive product decisions; those remain subject to the normal decision/conflict protocol.
- Reason: avoid unnecessary interruption while designing the project's documentation system.

## DEC-008 — Foundation engine: Godot 4.7.2 + GDScript
- Status: ACTIVE
- Date: 2026-09-10
- Decision: use **Godot 4.7.2 stable with GDScript** as the foundation engine for the prototype, targeting a stylized low-poly 3D world. Native desktop execution is the primary development/validation path; browser export remains a supported distribution/validation target rather than the constraint that determines the entire architecture.
- Reason: the approved product direction now requires procedural seeded worlds and scalable 3D exploration. Godot provides a complete 3D scene/node/input/physics/rendering/audio toolset without requiring us to build an engine. It also has official Web export support, including single-threaded Web export, while native desktop remains the stronger environment for developing and profiling the 3D prototype.
- Alternatives considered:
  - **Phaser + TypeScript:** excellent browser-first 2D framework, but Phaser is explicitly a 2D framework and does not provide built-in 3D rendering/physics; choosing it would force a major representation compromise or additional 3D technology.
  - **Three.js + TypeScript:** strong browser 3D rendering, but would leave substantially more game-engine responsibilities (scene/gameplay architecture, physics choices, tooling and content workflow) to the project. That increases custom infrastructure and agent-maintenance surface too early.
  - **Canvas + TypeScript without a 3D engine:** rejected as an engine foundation because the project would need to build core 3D/rendering/game systems itself.
- Consequences:
  - The first playable representation is 3D low-poly/stylized, not 2D top-down.
  - Procedural generation is treated as a first-class game system, but the first implementation must use a small bounded test world rather than an infinite world.
  - Game rules, seed data, world-generation algorithms, mission state and terminal simulation should remain separated from presentation nodes where practical.
  - GDScript is the project scripting language for the foundation; adding C# is not justified for the prototype, and Godot 4 C# is not compatible with Web export.
  - Browser support must be tested explicitly as the project grows because Web export has platform-specific limitations and performance trade-offs.
- Supersedes: the previous unapproved Phaser + TypeScript candidate recorded in `AGENTS/PROJECT_STATUS.md`.

## Decision template
For future decisions use:

### DEC-XXX — Title
- Status: PROPOSED | ACTIVE | SUPERSEDED
- Date: YYYY-MM-DD
- Decision:
- Reason:
- Alternatives considered:
- Consequences:
- Supersedes: (if applicable)
