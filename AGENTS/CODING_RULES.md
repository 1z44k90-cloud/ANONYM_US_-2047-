# CODING RULES

## Architecture
- Keep systems modular and testable.
- Separate world simulation, UI, terminal simulation, narrative state and persistence.
- Avoid putting game logic directly inside rendering code.
- Prefer data-driven missions and dialogue over hard-coded sequences.

## Code quality
- Use clear names.
- Keep functions small enough to understand quickly.
- Comment decisions and non-obvious behavior, not obvious syntax.
- Do not introduce a dependency unless it has a clear benefit.
- Preserve existing behavior unless a task explicitly changes it.

## Game-state discipline
Important state must have one authoritative owner. Avoid duplicated state between UI components and gameplay systems.

## Terminal sandbox
The terminal must operate only on an in-game virtual filesystem/network. No shell execution, real credentials, real network scanning, real malware, persistence mechanisms, or real-world exploit functionality.

## Performance
Target a lightweight browser/desktop experience first. Avoid unnecessary per-frame allocations and excessive DOM work.

## Accessibility
Keep important information readable. Do not make the terminal purely decorative: commands and responses must communicate meaningful gameplay information.

## Agent behavior
Before changing architecture, inspect the relevant documentation and existing code. Make the smallest coherent change that advances the current issue. Update documentation when a design decision changes.
