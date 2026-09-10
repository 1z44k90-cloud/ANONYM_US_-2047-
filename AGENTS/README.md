# AGENTS — DEVELOPMENT CONTROL CENTER

This directory contains the rules that coordinate human and AI development of ANONYM_US_<2047>.

## Read order

1. `MASTER_CONTEXT.md` — what the project is and what must not be contradicted.
2. `PROJECT_STATUS.md` — where the project currently is.
3. `DECISIONS.md` — decisions that are currently authoritative.
4. `TASK_PROTOCOL.md` — how work must be performed.
5. `CODING_RULES.md` — implementation constraints.
6. `PROMPTS/<task>.md` — exact scope of the assigned task.

## Core principle
**The repository must be understandable without the chat that created it.**

Conversation can provide intent and clarification, but durable project knowledge belongs in GitHub.

## Stable branch
`main` is the stable integrated state. Work happens in dedicated branches and reaches `main` through reviewable pull requests.

## Current control documents
- Master context: `MASTER_CONTEXT.md`
- Status: `PROJECT_STATUS.md`
- Decisions: `DECISIONS.md`
- Task protocol: `TASK_PROTOCOL.md`
- Coding rules: `CODING_RULES.md`
- Task prompts: `PROMPTS/`
