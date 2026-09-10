# TASK 25 — AUDITORÍA DE DOCUMENTACIÓN

## Objective
Verify that the documentation-control system remains internally consistent after governance changes.

## Checks
- [ ] Master context identifies the source-of-truth hierarchy.
- [ ] Project status identifies one current phase and next task.
- [ ] Decision log contains active governance decisions.
- [ ] Task protocol defines branch, conflict, testing and handoff rules.
- [ ] Prompts are Markdown and use bounded scopes.
- [ ] No prompt instructs agents to work directly on `main`.
- [ ] Current documentation does not claim unimplemented architecture is complete.
- [ ] Safety boundaries remain explicit.

## Acceptance criteria
All contradictions found are resolved or documented as blockers before the documentation system is considered stable.
