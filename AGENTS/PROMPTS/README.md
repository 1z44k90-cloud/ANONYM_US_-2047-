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
- `00_AGENT_BOOTSTRAP.md` — enter/review project context before work.
- `01_FOUNDATION_STACK.md` — technical stack decision.
- `02_PLAYER_MOVEMENT.md` — executable foundation.
- `03_TERMINAL_ENGINE.md` — fictional terminal engine.
- `04_VERTICAL_SLICE.md` — first complete gameplay loop.
- `05_HANDOFF.md` — required closing/handoff structure.
- `06_REVIEW_CHECKLIST.md` — pre-merge review checklist.
- `07_PHASE_TRANSITION.md` — phase completion/transition procedure.
- `08_AGENT_TASK_TEMPLATE.md` — reusable task template.
- `09_REPOSITORY_CONSISTENCY_AUDIT.md` — periodic consistency audit.
- `10_ISSUE_TO_PROMPT_WORKFLOW.md` — issue-to-agent-task workflow.
- `11_DOCUMENTATION_CHANGE.md` — documentation-only changes.
- `12_BUGFIX.md` — controlled bug fixes.
- `13_FEATURE.md` — bounded feature implementation.
- `14_TEST_AND_REGRESSION.md` — test/regression work.
- `15_ARCHITECTURE_CHANGE.md` — architecture changes.
- `16_RELEASE_READINESS.md` — release readiness checks.
- `17_AGENT_RESEARCH.md` — research before a decision.
- `18_DATA_CONTENT.md` — data-driven content.
- `19_SAVE_STATE.md` — persistence.
- `20_INTEGRATION.md` — system integration.
- `21_SCOPE_REVIEW.md` — scope review.
- `22_PRE_MERGE.md` — pre-merge validation.
- `23_CHANGELOG.md` — meaningful project history.
- `24_GITHUB_PR.md` — pull request definition.
- `25_DOCUMENTATION_AUDIT.md` — documentation governance audit.
