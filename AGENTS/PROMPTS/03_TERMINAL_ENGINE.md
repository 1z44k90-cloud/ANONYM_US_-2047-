# TASK 03 — TERMINAL ENGINE FICTICIO

## Objective
Implement the minimum closed fictional terminal system required by the vertical slice.

## Context
The terminal is a gameplay interface, not a real shell. It must simulate commands, files, credentials, networks and payload behavior entirely inside game state.

## Required reading
- `AGENTS/MASTER_CONTEXT.md`
- `AGENTS/PROJECT_STATUS.md`
- `AGENTS/DECISIONS.md`
- `AGENTS/TASK_PROTOCOL.md`
- `TECH/TERMINAL_ENGINE.md`
- `DESIGN/TERMINAL.md`
- `TECH/SECURITY_BOUNDARIES.md`

## Allowed files
- Terminal engine implementation
- Terminal-related tests
- Directly related terminal documentation

## Forbidden files
- Host OS shell execution
- Real network connections/scanning
- Real credentials
- Real malware/exploits/persistence
- Player movement implementation unless an explicit interface is required
- Unrelated narrative or world systems

## Preconditions
- Technical stack is selected.
- Project shell runs locally.
- Terminal contracts in technical/design documentation are understood.

## Task
Implement a minimal virtual terminal with data-driven fictional state and a command parser sufficient for the vertical slice. Initial commands may include `help`, `ls`, `cd`, `cat`, `scan`, `connect`, `grep` and `decrypt`, but all behavior must be simulated.

Commands must operate only on an in-memory or game-owned virtual filesystem/network. No host shell, filesystem or network API may be used for gameplay actions.

## Acceptance criteria
- Terminal opens inside the game.
- Supported fictional commands produce deterministic game-state responses.
- Invalid commands fail safely.
- Virtual files/network nodes can be queried without touching the host OS.
- Terminal state is isolated from real system resources.
- Tests cover parser behavior and core command safety.

## Tests
- Automated/unit tests for command parsing and virtual state.
- Manual test of opening terminal and running supported/invalid commands.
- Verify no real OS/network side effects are possible.

## Documentation updates
Update terminal technical/design documentation and `AGENTS/PROJECT_STATUS.md` as required.

## Handoff
Report implemented commands, virtual-state model, tests, known limitations and the next integration task.
