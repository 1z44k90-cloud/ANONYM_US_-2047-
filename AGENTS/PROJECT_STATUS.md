# PROJECT STATUS — ANONYM_US_<2047>

## Purpose
Single visible status board for the project. Any agent must read this file before starting work and update it when a task changes project state.

## Current phase
**FASE 1 — FUNDACIÓN TÉCNICA**

### Phase state
- Status: 🔄 ACTIVE
- Objective: establish a stable development process, technical foundation and playable prototype path.
- Current priority: resolve the technical stack and then begin the smallest executable foundation.
- Current blockers: technical stack decision is pending.

## Phases

| Phase | Status | Objective |
|---|---|---|
| FASE 0 — PRE-PRODUCCIÓN | ✅ COMPLETE | Vision, world, narrative direction and initial architecture documented. |
| FASE 1 — FUNDACIÓN TÉCNICA | 🔄 ACTIVE | Lock workflow, stack and project foundation. |
| FASE 2 — VERTICAL SLICE | ⏳ PENDING | Prove the core gameplay loop in a small Tijuana district. |
| FASE 3 — SISTEMAS CORE | ⏳ PENDING | Expand validated gameplay systems. |
| FASE 4 — MUNDO | ⏳ PENDING | Build the broader playable world. |
| FASE 5 — NARRATIVA | ⏳ PENDING | Integrate full narrative, missions and character arcs. |
| FASE 6 — POLISH | ⏳ PENDING | Performance, UX, audio, visuals, accessibility and stability. |
| FASE 7 — RELEASE | ⏳ PENDING | Packaging, QA, deployment and release preparation. |

## Active work
1. Development governance and agent documentation — prepared on `docs/agent-development-system`.
2. Technical stack decision — next implementation decision.
3. After stack approval: executable project shell and player movement.

## Next task
**TASK 01 — DEFINIR STACK TÉCNICO DEL PROTOTIPO** (`AGENTS/PROMPTS/01_FOUNDATION_STACK.md`)

Current candidate: Phaser + TypeScript. This is a candidate, not yet an approved architectural decision.

## Dependencies
`TASK 01` must be resolved before `TASK 02 — PLAYER MOVEMENT`.

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
