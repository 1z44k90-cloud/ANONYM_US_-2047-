# CODING RULES — ANONYM_US_<2047>

## Architecture
- Keep systems modular and testable.
- Separate world simulation, UI, terminal simulation, narrative state and persistence.
- Avoid putting game logic directly inside rendering code.
- Prefer data-driven missions and dialogue over hard-coded sequences.
- Keep important state under one authoritative owner.
- Use explicit interfaces/events between systems instead of hidden coupling.

## Scope
- Implement the smallest coherent solution that advances the current task.
- Do not add speculative systems merely because they may be useful later.
- Do not introduce a dependency unless it has a clear, documented benefit.
- Preserve existing behavior unless the task explicitly changes it.

## Code quality
- Use clear names.
- Keep functions small enough to understand quickly.
- Comment decisions and non-obvious behavior, not obvious syntax.
- Prefer predictable, maintainable patterns over clever abstractions.

## Game-state discipline
Important state must have one authoritative owner. Avoid duplicated state between UI components and gameplay systems.

## Terminal sandbox
The terminal must operate only on an in-game virtual filesystem/network. No shell execution, real credentials, real network scanning, real malware, persistence mechanisms, or real-world exploit functionality.

## Performance
Target a lightweight browser/desktop experience first. Avoid unnecessary per-frame allocations and excessive DOM work.

## Accessibility
Keep important information readable. Do not make the terminal purely decorative: commands and responses must communicate meaningful gameplay information.

## Testing
Every implementation must have an appropriate verification method. Prefer automated tests where practical, supplemented by manual gameplay verification for visual/input/runtime behavior.

## Agent behavior
Before changing architecture, inspect `AGENTS/MASTER_CONTEXT.md`, `AGENTS/PROJECT_STATUS.md`, `AGENTS/DECISIONS.md` and relevant code. Follow `AGENTS/TASK_PROTOCOL.md`. Never silently contradict an active decision. Update documentation when design, behavior or architecture changes.
