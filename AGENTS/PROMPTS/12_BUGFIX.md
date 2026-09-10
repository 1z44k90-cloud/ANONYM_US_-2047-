# TASK 12 — BUGFIX CONTROLADO

## Objective
Fix one reproducible defect without expanding scope or introducing unrelated refactors.

## Required reading
- `AGENTS/MASTER_CONTEXT.md`
- `AGENTS/PROJECT_STATUS.md`
- `AGENTS/DECISIONS.md`
- `AGENTS/TASK_PROTOCOL.md`
- relevant system documentation
- GitHub issue describing the defect

## Preconditions
- The bug is reproducible or there is sufficient evidence to define expected behavior.
- The owning system is identified.

## Task
1. Reproduce the defect.
2. Identify the smallest root cause.
3. Implement the smallest coherent fix.
4. Add or update a regression test when practical.
5. Re-test the affected system and relevant adjacent behavior.

## Scope rules
- Do not perform broad refactors under a bugfix task.
- Do not change architecture unless the bug proves the existing architecture is impossible; use the conflict protocol if so.
- Do not hide unrelated changes inside the fix.

## Acceptance criteria
- Original defect no longer reproduces.
- Regression coverage exists when practical.
- No critical regression is introduced.
- Documentation is updated if expected behavior changed.

## Handoff
Report reproduction, root cause, fix, tests, files changed and remaining limitations.
