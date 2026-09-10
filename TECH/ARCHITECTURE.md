# ARCHITECTURE

## Target
Browser-first prototype that can later be packaged for desktop if the vertical slice succeeds.

## Major systems
- **World** — map, entities, movement, interaction.
- **Renderer** — 2D scene and effects.
- **Game State** — authoritative runtime state.
- **Mission Engine** — objectives, triggers, consequences.
- **Terminal Engine** — fictional filesystem/network and command parser.
- **Dialogue Engine** — conversations, branching and flags.
- **AI Director** — narrative threat reactions, not real AI model control.
- **Persistence** — save/load progression.
- **UI** — HUD, terminal, dialogue and menus.

## Dependency direction
Rendering/UI should consume state rather than own core gameplay state. Mission and dialogue systems should communicate through explicit events/flags. The terminal engine must remain isolated from the host operating system.

## First implementation order
1. Project shell.
2. 2D world and movement.
3. Interaction system.
4. Terminal engine.
5. Mission state machine.
6. Dialogue/Julia.
7. Detection/trace system.
8. Save state.
9. Vertical-slice polish.
