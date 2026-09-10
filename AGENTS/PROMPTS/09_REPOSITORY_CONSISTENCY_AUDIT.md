# TASK 09 — REPOSITORY CONSISTENCY AUDIT

## Objective
Audit the repository documentation and implementation for contradictions before a major phase transition.

## Required reading
- `AGENTS/MASTER_CONTEXT.md`
- `AGENTS/PROJECT_STATUS.md`
- `AGENTS/DECISIONS.md`
- `AGENTS/TASK_PROTOCOL.md`
- `AGENTS/CODING_RULES.md`
- all documentation directly related to the systems being audited

## Procedure
Check for:
- contradictory architecture decisions;
- obsolete phase/status information;
- duplicated or conflicting rules;
- task prompts that exceed current scope;
- undocumented implementation changes;
- safety-boundary violations;
- references to files that no longer exist;
- missing next-task definitions.

## Rule
Do not silently rewrite a disputed decision. Report the contradiction, identify its sources and resolve it through the decision protocol.

## Acceptance criteria
- All identified inconsistencies are either resolved or explicitly documented as blockers.
- Status reflects reality.
- No known critical documentation contradiction remains.

## Handoff
Provide an audit summary and list the next corrective tasks in priority order.
