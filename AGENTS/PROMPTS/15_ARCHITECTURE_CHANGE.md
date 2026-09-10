# TASK 15 — CAMBIO ARQUITECTÓNICO

## Objective
Change a project-wide technical architecture decision only when the current architecture no longer satisfies a demonstrated requirement.

## Required reading
- `AGENTS/MASTER_CONTEXT.md`
- `AGENTS/PROJECT_STATUS.md`
- `AGENTS/DECISIONS.md`
- `AGENTS/TASK_PROTOCOL.md`
- affected `TECH/` documentation
- relevant GitHub issue

## Preconditions
A concrete limitation, requirement or validated evidence justifies revisiting the architecture.

## Task
1. Describe the current architecture and limitation.
2. Identify affected systems.
3. Evaluate alternatives.
4. Define migration impact.
5. Record the decision in `AGENTS/DECISIONS.md`.
6. Update the master/technical documentation.
7. Only then implement migration work in separate, bounded tasks when practical.

## Rule
Do not use a feature task to smuggle in an architectural rewrite.

## Acceptance criteria
- The reason for change is explicit.
- Alternatives were considered.
- Decision log and technical documentation agree.
- Migration scope is understood.
- Existing functionality is not silently abandoned.

## Handoff
Report current architecture, reason for change, chosen alternative, affected systems, migration plan and next implementation task.
