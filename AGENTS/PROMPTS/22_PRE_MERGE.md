# TASK 22 — PRE-MERGE VALIDATION

## Objective
Validate a branch before opening or approving a pull request into `main`.

## Required reading
- `AGENTS/MASTER_CONTEXT.md`
- `AGENTS/PROJECT_STATUS.md`
- `AGENTS/DECISIONS.md`
- `AGENTS/TASK_PROTOCOL.md`
- assigned task prompt
- `AGENTS/PROMPTS/06_REVIEW_CHECKLIST.md`

## Procedure
1. Compare branch changes against `main`.
2. Confirm all changes belong to the assigned task.
3. Run required tests.
4. Review documentation synchronization.
5. Check for architectural/scope/security regressions.
6. Confirm handoff is complete.

## Acceptance criteria
- Diff matches task scope.
- Required tests pass.
- Review checklist has no unresolved mandatory item.
- PR description can accurately state what was verified.

## Rule
Do not approve a branch simply because it compiles. The change must satisfy the task's actual acceptance criteria.
