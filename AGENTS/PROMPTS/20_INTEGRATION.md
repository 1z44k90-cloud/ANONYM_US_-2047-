# TASK 20 — INTEGRACIÓN ENTRE SISTEMAS

## Objective
Connect two already validated systems through an explicit, minimal interface.

## Required reading
- `AGENTS/MASTER_CONTEXT.md`
- `AGENTS/PROJECT_STATUS.md`
- `AGENTS/DECISIONS.md`
- `AGENTS/TASK_PROTOCOL.md`
- documentation for both systems
- GitHub issue

## Preconditions
Both systems work independently and their authoritative state owners are known.

## Task
Define the smallest explicit contract needed for integration. Prefer events, commands or typed state transitions over direct hidden dependencies.

## Acceptance criteria
- Contract is documented.
- Each system retains ownership of its own state.
- Integration is testable.
- No circular dependency is introduced.
- Existing standalone behavior remains intact unless explicitly changed.

## Handoff
Report the interface/contract, files changed, tests, dependencies and next integration step.
