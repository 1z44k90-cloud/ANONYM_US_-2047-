# TASK 21 — REVISIÓN DE ALCANCE

## Objective
Evaluate whether a proposed feature belongs in the current phase before implementation begins.

## Required reading
- `AGENTS/MASTER_CONTEXT.md`
- `AGENTS/PROJECT_STATUS.md`
- `AGENTS/DECISIONS.md`
- `ROADMAP.md`
- relevant design/technical documentation
- proposed GitHub issue

## Questions
- Does it support the current phase objective?
- Does it validate or strengthen the core loop?
- What existing systems does it affect?
- What dependencies does it introduce?
- Can it be deferred without harming the vertical slice?
- What is the smallest version worth implementing?

## Rule
Prefer deferral over premature complexity when the feature does not materially improve the current validation milestone.

## Acceptance criteria
The issue receives one of: `NOW`, `DEFER`, or `REVISE`, with a documented reason and next action.

## Handoff
Record the scope decision and update project status/roadmap if the decision changes priorities.
