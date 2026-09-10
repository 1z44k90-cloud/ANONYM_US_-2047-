# DECISIONS — ANONYM_US_<2047>

This is the architectural and process decision log. Decisions recorded here are authoritative until explicitly superseded.

## DEC-001 — Agent development workflow
- Status: ACTIVE
- Decision: AI agents must use a controlled loop: READ → PLAN → IMPLEMENT → TEST → REVIEW → DOCUMENT → UPDATE STATUS → HANDOFF.
- Reason: prevent duplicated work, contradictory changes and unfinished handoffs.
- Consequence: an agent is not finished when code merely exists; it must leave a tested, documented and understandable state.

## DEC-002 — `main` is the stable branch
- Status: ACTIVE
- Decision: `main` represents the latest approved/integrated project state. Agents must not use `main` as their normal working branch.
- Workflow: task `.md` → feature branch → implementation/tests/review → pull request → merge to `main`.
- Reason: preserve a reliable baseline and make changes auditable.
- Consequence: experimental or incomplete work stays outside `main`.

## DEC-003 — Documentation is part of the product source of truth
- Status: ACTIVE
- Decision: project intent, architecture, process, phase status and important decisions must live in version-controlled repository documentation.
- Reason: future agents need durable context that does not depend on conversation history.
- Consequence: undocumented architectural changes are considered incomplete.

## DEC-004 — One coherent system per agent task
- Status: ACTIVE
- Decision: an agent owns one coherent area per task and communicates with other systems through explicit interfaces/state.
- Reason: reduce hidden coupling and conflicting edits.
- Consequence: an agent must not redesign another system silently.

## DEC-005 — Architectural conflict protocol
- Status: ACTIVE
- Decision: when an assigned task conflicts with an existing decision, the agent must stop before expanding the conflicting implementation, document the conflict and propose a resolution.
- Reason: prevent silent architectural drift.
- Consequence: the master context and decision log remain internally consistent.

## DEC-006 — Terminal/network safety boundary
- Status: ACTIVE
- Decision: all terminal, credentials, malware, exploits and network behavior are fictional game mechanics isolated from the host operating system.
- Reason: preserve the game's design while preventing real-world operational functionality.
- Consequence: no real unauthorized-access or malware functionality belongs in the game code.

## Decision template
For future decisions use:

### DEC-XXX — Title
- Status: PROPOSED | ACTIVE | SUPERSEDED
- Date: YYYY-MM-DD
- Decision:
- Reason:
- Alternatives considered:
- Consequences:
- Supersedes: (if applicable)
