# PROJECT STATUS — ANONYM_US_<2047>

## Purpose
Single visible status board for the project. Any agent must read this file before starting work and update it when a task changes project state.

## Current phase
**FASE 1 — FUNDACIÓN TÉCNICA**

### Phase state
- Status: 🔄 ACTIVE
- Objective: establish a stable development process, technical foundation and playable prototype path.
- Current priority: finalize the development protocol and technical stack before building large systems.
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
1. Formalize agent workflow and branch policy.
2. Maintain documentation as the source of truth.
3. Resolve the technical stack decision.
4. Then implement the smallest playable foundation.

## Next task
**Resolve technical stack for the browser-first vertical slice.**

Candidate under evaluation: Phaser + TypeScript.

The stack must be documented in `TECH/ARCHITECTURE.md` and `AGENTS/DECISIONS.md` before major implementation begins.

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
