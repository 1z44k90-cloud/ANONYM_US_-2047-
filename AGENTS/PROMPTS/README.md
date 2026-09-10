# PROMPTS — TASK SPECIFICATIONS

All official agent task prompts must be Markdown (`.md`) files stored in this directory.

## Required prompt structure

Every task prompt should contain:

1. **Objective** — exactly what must be achieved.
2. **Context** — why the task exists and relevant project constraints.
3. **Required reading** — master context, status, issue and related technical/design documents.
4. **Allowed files** — files the agent may modify.
5. **Forbidden files** — files/systems the agent must not modify without explicit approval.
6. **Preconditions** — what must already be true before work begins.
7. **Implementation task** — smallest useful implementation.
8. **Acceptance criteria** — observable conditions that prove completion.
9. **Tests** — commands or checks required before handoff.
10. **Documentation updates** — documents that must be updated if behavior/design changes.
11. **Handoff** — what the next agent needs to know.

## Prompt naming
Use:

`NN_SYSTEM_TASK.md`

Examples:
- `01_FOUNDATION_STACK.md`
- `02_PLAYER_MOVEMENT.md`
- `03_TERMINAL_ENGINE.md`

## Scope rule
A prompt should be small enough that one agent can complete, test and document it without redesigning unrelated systems.

## Branch rule
The agent works on a dedicated feature/docs branch. The prompt must never instruct an agent to commit directly to `main`.

## Completion rule
A prompt is complete only when its acceptance criteria and required tests pass and the handoff is documented.

## Standard templates
- `08_AGENT_TASK_TEMPLATE.md` — copy this for new implementation/documentation tasks.
- `05_HANDOFF.md` — required closing/handoff structure.
- `06_REVIEW_CHECKLIST.md` — pre-merge review checklist.
- `07_PHASE_TRANSITION.md` — phase completion/transition procedure.
- `09_REPOSITORY_CONSISTENCY_AUDIT.md` — periodic consistency audit.
