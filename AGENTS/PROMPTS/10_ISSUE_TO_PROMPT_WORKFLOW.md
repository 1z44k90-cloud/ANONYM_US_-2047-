# TASK 10 — ISSUE → PROMPT → BRANCH → PR WORKFLOW

## Objective
Standardize how GitHub issues become executable agent tasks.

## Workflow
1. Create or select one GitHub issue for a coherent outcome.
2. Create the corresponding `.md` prompt in `AGENTS/PROMPTS/`.
3. Define scope, allowed/forbidden files, prerequisites, acceptance criteria and tests.
4. Confirm the task is compatible with `PROJECT_STATUS.md` and `DECISIONS.md`.
5. Create a dedicated branch.
6. Agent executes the controlled loop from `TASK_PROTOCOL.md`.
7. Review the resulting diff against the prompt and review checklist.
8. Open a pull request into `main`.
9. Merge only after the task is actually verified.
10. Update project status and close the issue when appropriate.

## Rule
One issue should describe the outcome; the prompt describes how an agent is constrained to achieve that outcome. Do not use an issue as a substitute for durable project architecture documentation.

## Acceptance criteria
A task is ready for implementation only when another agent can execute the prompt without needing hidden context from the original conversation.
