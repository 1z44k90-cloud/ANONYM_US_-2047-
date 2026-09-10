# TASK 00 — AGENT BOOTSTRAP / REVISIÓN DE CONTEXTO

## Objective
Ensure an agent can enter the project without relying on prior conversation history and can identify the correct next task.

## Required reading
1. `AGENTS/MASTER_CONTEXT.md`
2. `AGENTS/PROJECT_STATUS.md`
3. `AGENTS/DECISIONS.md`
4. `AGENTS/TASK_PROTOCOL.md`
5. `AGENTS/CODING_RULES.md`
6. assigned task prompt, if applicable

## Procedure
- Identify the current phase.
- Identify the active task and blockers.
- Identify the relevant GitHub issue.
- Check active architectural decisions.
- Inspect the relevant code before proposing changes.
- Confirm the task does not conflict with the current project state.

## Rule
This is a preparation/checkpoint prompt, not permission to modify unrelated systems.

## Output
The agent should be able to state:
- current phase;
- current objective;
- active blockers;
- assigned scope;
- files allowed to change;
- tests required;
- next handoff target.
