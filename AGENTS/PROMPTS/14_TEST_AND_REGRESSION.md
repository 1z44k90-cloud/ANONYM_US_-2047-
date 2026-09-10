# TASK 14 — TEST Y REGRESIÓN

## Objective
Verify a system or vertical slice after a change and detect regressions before integration.

## Required reading
- `AGENTS/MASTER_CONTEXT.md`
- `AGENTS/PROJECT_STATUS.md`
- `AGENTS/DECISIONS.md`
- `AGENTS/TASK_PROTOCOL.md`
- relevant system documentation

## Task
Run the project's available automated and manual verification relevant to the changed system. Add regression coverage where a stable automated check is practical.

## Acceptance criteria
- Required verification is executed, not merely planned.
- Results are recorded accurately.
- Any failure is either fixed or documented as a blocker.
- No critical known regression is ignored.

## Rule
Never report a test as passing if it was not actually executed.

## Handoff
Report commands/checks, results, failures, fixes and remaining risks.
