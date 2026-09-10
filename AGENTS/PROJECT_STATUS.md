# PROJECT STATUS — ANONYM_US_<2047>

## Purpose
Single visible status board for the project. Any agent must read this file before starting work and update it when a task changes project state.

## Current phase
**FASE 1 — FUNDACIÓN TÉCNICA**

### Phase state
- Status: 🔄 ACTIVE
- Objective: establish a stable development process, technical foundation and playable prototype path.
- Current priority: build the smallest executable Godot foundation and validate deterministic seeded 3D world generation.
- Current blockers: executable project shell does not exist yet.

## Phases

| Phase | Status | Objective |
|---|---|---|
| FASE 0 — PRE-PRODUCCIÓN | ✅ COMPLETE | Vision, world, narrative direction and initial architecture documented. |
| FASE 1 — FUNDACIÓN TÉCNICA | 🔄 ACTIVE | Lock workflow, stack and project foundation. |
| FASE 2 — VERTICAL SLICE | ⏳ PENDING | Prove the core gameplay loop in a small generated world. |
| FASE 3 — SISTEMAS CORE | ⏳ PENDING | Expand validated gameplay systems. |
| FASE 4 — MUNDO | ⏳ PENDING | Expand procedural world generation and runtime streaming only after validation. |
| FASE 5 — NARRATIVA | ⏳ PENDING | Integrate full narrative, missions and character arcs. |
| FASE 6 — POLISH | ⏳ PENDING | Performance, UX, audio, visuals, accessibility and stability. |
| FASE 7 — RELEASE | ⏳ PENDING | Packaging, QA, deployment and release preparation. |

## Active work
1. Development governance and agent documentation — integrated on `main`.
2. TASK 01 — technical stack decision — resolved on `task/01-foundation-stack`.
3. TASK 02 — executable Godot project shell + smallest deterministic seeded 3D test world — next.

## Technical foundation
- Engine: **Godot 4.7.2 stable**.
- Scripting: **GDScript**.
- Representation: **stylized low-poly 3D**.
- World: **deterministic procedural generation from seeds**.
- Development target: native desktop first; Web export supported and validated progressively.
- Terminal: closed fictional simulation only.

## Next task
**TASK 02 — PROJECT SHELL + SEEDED 3D FOUNDATION** (`AGENTS/PROMPTS/02_PLAYER_MOVEMENT.md`)

TASK 02 must be updated before implementation if its old 2D assumptions conflict with DEC-008. The task should establish the executable Godot project, a small deterministic generated test area, player movement, camera and basic collision/bounds without expanding into a large world.

## Dependencies
`TASK 02` depends on `TASK 01` and must precede terminal/gameplay implementation.

## Definition of Done for FASE 1
- Agent workflow documented.
- Branch/PR policy documented.
- Prompt format documented.
- Conflict/decision protocol documented.
- Technical stack selected and recorded.
- Project can be started locally with documented commands.
- First implementation task has explicit acceptance criteria and tests.

## Update protocol
Every meaningful task completion must update:
- this file when phase/progress/next task changes;
- `AGENTS/DECISIONS.md` for architectural decisions;
- relevant technical/design documentation when behavior changes.

Do not mark a phase complete based only on documentation. Its Definition of Done must be satisfied.
