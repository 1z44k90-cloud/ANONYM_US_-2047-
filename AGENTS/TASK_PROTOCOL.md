# TASK PROTOCOL — ANONYM_US_<2047>

## Mandatory pre-work
Before modifying anything, an agent must:

1. Read `AGENTS/MASTER_CONTEXT.md`.
2. Read `AGENTS/PROJECT_STATUS.md`.
3. Read the assigned task prompt in `AGENTS/PROMPTS/` when one exists.
4. Read the linked GitHub issue.
5. Read documentation directly related to the task.
6. Inspect the existing implementation before proposing replacements.
7. Check whether the proposed work conflicts with an active decision in `AGENTS/DECISIONS.md`.

## Controlled agent loop
Every implementation task follows this loop:

`READ → PLAN → IMPLEMENT → TEST → REVIEW → DOCUMENT → UPDATE STATUS → HANDOFF`

The loop is finite and controlled by the task's acceptance criteria. If a test fails, fix and retest until the exit criteria are met or the blocker is documented.

## Scope discipline
- One agent owns one coherent system/area per task.
- Modify only files explicitly allowed by the task, plus directly necessary documentation.
- Do not redesign unrelated systems to solve a local problem.
- Prefer small, reversible changes during prototype development.
- Existing behavior should remain intact unless the task explicitly changes it.

## Conflict protocol
If the task conflicts with existing architecture, narrative, security boundaries or another active decision:

1. Stop before implementing the conflicting design.
2. Identify the exact conflicting documents/decisions.
3. Explain the conflict and its practical consequence.
4. Propose the smallest resolution or alternatives.
5. Record the decision in `AGENTS/DECISIONS.md` if it is architectural or process-level.
6. Update affected documentation so there is one consistent source of truth.
7. Continue only after the conflict is resolved.

Never silently overwrite an established decision.

## Branch and `main` policy
`main` is the stable/integrated branch.

Agents work on dedicated branches named for the scope, for example:
- `feature/player-movement`
- `feature/terminal-engine`
- `feature/dialogue-system`
- `docs/agent-development-system`

Normal flow:

`task prompt → branch → implement → test → review → pull request → merge → main`

An agent must not use `main` as its normal working branch or treat unreviewed work as stable.

## Prompt requirement
Official agent instructions must be stored as Markdown files under `AGENTS/PROMPTS/`.

Each prompt should define:
- Objective
- Context
- Required reading
- Allowed files
- Forbidden files
- Preconditions
- Implementation task
- Acceptance criteria
- Tests
- Documentation updates
- Handoff

See `AGENTS/PROMPTS/README.md`.

## Testing requirement
A task must state how it will be tested. Depending on scope this may include:
- automated tests;
- type checking/build;
- linting;
- local runtime verification;
- manual gameplay verification;
- regression checks.

Do not claim a task is tested if only the code was inspected.

## Documentation requirement
Update documentation when a task changes:
- architecture;
- public interfaces/contracts;
- gameplay behavior;
- controls;
- data formats;
- security boundaries;
- development workflow;
- phase status;
- important decisions.

## Handoff requirement
Every completed task must report:
- what changed;
- files changed;
- tests executed and results;
- known limitations;
- decisions made;
- next recommended task;
- anything another agent must know before continuing.

## Definition of Done
A task is complete only when:
- acceptance criteria pass;
- required tests pass;
- no known critical regression remains;
- documentation is synchronized;
- project status is updated when necessary;
- handoff information is available.
