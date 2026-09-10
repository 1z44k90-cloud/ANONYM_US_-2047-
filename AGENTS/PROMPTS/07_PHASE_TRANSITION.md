# TASK 07 — PHASE TRANSITION

## Objective
Prevent the project from advancing phases merely because a few tasks are complete.

## Required reading
- `AGENTS/MASTER_CONTEXT.md`
- `AGENTS/PROJECT_STATUS.md`
- `AGENTS/DECISIONS.md`
- `AGENTS/TASK_PROTOCOL.md`

## Procedure
Before changing the active phase, verify the current phase Definition of Done item by item.

Record:
- completed criteria;
- evidence/tests;
- unresolved limitations;
- new phase objective;
- first task of the new phase.

Update `AGENTS/PROJECT_STATUS.md` and, when the transition represents a durable architectural/process decision, `AGENTS/DECISIONS.md`.

## Rule
If one required criterion is not satisfied, keep the current phase active and document the blocker.

## Handoff
The next agent must be able to identify the new phase, its objective, current blockers and exact first task without relying on chat history.
