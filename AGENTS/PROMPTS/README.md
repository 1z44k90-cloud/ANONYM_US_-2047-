# PROMPTS — TASK SPECIFICATIONS

All official agent task prompts must be Markdown (`.md`) files stored in this directory.

## Required prompt structure
Every task prompt should contain Objective, Context, Required reading, Allowed files, Forbidden files, Preconditions, Implementation task, Acceptance criteria, Tests, Documentation updates and Handoff.

## Naming
Use `NN_SYSTEM_TASK.md`.

## Scope
A prompt must be small enough for one agent to complete, test and document without redesigning unrelated systems.

## Branch rule
Agents work on dedicated feature/docs branches and never directly on `main`.

## Standard prompts/templates
- `00_AGENT_BOOTSTRAP.md` — context checkpoint.
- `01_FOUNDATION_STACK.md` — technical stack decision.
- `02_PLAYER_MOVEMENT.md` — executable foundation.
- `03_TERMINAL_ENGINE.md` — fictional terminal engine.
- `04_VERTICAL_SLICE.md` — first complete gameplay loop.
- `05_HANDOFF.md` — handoff standard.
- `06_REVIEW_CHECKLIST.md` — pre-merge review.
- `07_PHASE_TRANSITION.md` — phase transition.
- `08_AGENT_TASK_TEMPLATE.md` — reusable task template.
- `09_REPOSITORY_CONSISTENCY_AUDIT.md` — consistency audit.
- `10_ISSUE_TO_PROMPT_WORKFLOW.md` — issue-to-task flow.
- `11_DOCUMENTATION_CHANGE.md` — documentation-only task.
- `12_BUGFIX.md` — controlled bugfix.
- `13_FEATURE.md` — bounded feature.
- `14_TEST_AND_REGRESSION.md` — testing.
- `15_ARCHITECTURE_CHANGE.md` — architecture change.
- `16_RELEASE_READINESS.md` — release readiness.
- `17_AGENT_RESEARCH.md` — research before decision.
- `18_DATA_CONTENT.md` — data-driven content.
- `19_SAVE_STATE.md` — persistence.
- `20_INTEGRATION.md` — system integration.
- `21_SCOPE_REVIEW.md` — scope review.
- `22_PRE_MERGE.md` — pre-merge validation.
- `23_CHANGELOG.md` — project history.
- `24_GITHUB_PR.md` — PR definition.
- `25_DOCUMENTATION_AUDIT.md` — documentation governance audit.
- `26_GOVERNANCE_COMPLETE.md` — governance completion checkpoint.
- `27_GOVERNANCE_REVIEW.md` — final governance review.
- `28_DOCUMENTATION_RELEASE.md` — documentation release checkpoint.
- `29_NO_DIRECT_MAIN.md` — main branch protection.
- `30_DONE_DEFINITION.md` — universal definition of done.
- `31_DOCUMENTATION_GOVERNANCE.md` — documentation governance.
- `32_AGENT_HANDOFF.md` — mandatory handoff.
- `33_DOCUMENTATION_SYNC.md` — documentation synchronization.
