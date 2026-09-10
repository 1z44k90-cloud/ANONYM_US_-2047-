# TASK 13 — NUEVA FEATURE CONTROLADA

## Objective
Add one validated gameplay feature without allowing scope to expand into unrelated systems.

## Required reading
- `AGENTS/MASTER_CONTEXT.md`
- `AGENTS/PROJECT_STATUS.md`
- `AGENTS/DECISIONS.md`
- `AGENTS/TASK_PROTOCOL.md`
- relevant design/technical documentation
- GitHub issue for the feature

## Preconditions
- The feature has a defined gameplay purpose.
- The feature belongs to the current project phase.
- Dependencies and owning system are identified.

## Task
Implement the smallest version that can be validated in gameplay. Prefer data-driven state and explicit interfaces. Defer polish, scale and speculative extensions unless they are required for validation.

## Acceptance criteria
- The feature fulfills its defined gameplay purpose.
- It integrates through documented interfaces/state.
- Tests/verification pass.
- Scope remains within the assigned issue.
- Documentation is synchronized.

## Review questions
- Does this feature improve the validated core loop?
- Can it be removed or changed without destabilizing unrelated systems?
- Did it introduce unnecessary dependencies?
- Did it create duplicated authoritative state?
- Did it accidentally expand the project scope?

## Handoff
Report implementation, verification, design impact, known limitations and the next validation step.
