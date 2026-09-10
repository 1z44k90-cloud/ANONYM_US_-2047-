# ARCHITECTURE

## Target
A stylized, procedural post-apocalyptic sandbox with worlds generated from deterministic seeds. The first implementation is a small bounded 3D test world that can later scale toward larger streamed worlds if the vertical slice proves the concept.

The world is inspired by advanced contemporary cities and their infrastructure, but is not tied to a single real-world city. The post-apocalyptic identity comes from the contrast between advanced systems and a civilization that has collapsed or fragmented. Some infrastructure may remain operational under SYNAPSE's influence.

Native desktop execution is the primary development and profiling path. Browser export remains a supported target and must be validated during development, but browser constraints must not force the project back into a 2D representation.

## Foundation stack
- **Engine:** Godot 4.7.2 stable.
- **Primary scripting language:** GDScript.
- **Primary representation:** stylized low-poly 3D.
- **World model:** deterministic procedural generation from a seed.
- **Version control:** Git/GitHub.
- **Browser target:** Godot Web export, initially single-threaded unless profiling proves thread support necessary and hosting requirements are acceptable.

Godot was selected because the approved direction now depends on 3D exploration and procedural worlds. It provides the core 3D runtime, scene system, input, physics, rendering, audio and editor tooling without requiring the project to build a custom engine. Godot also supports Web export, so the browser remains viable without dictating the entire architecture.

## Major systems
- **World Generator** — deterministic seed → terrain, districts, roads, structures, points of interest and world-state parameters.
- **World Runtime** — loaded/generated chunks or regions, entities, movement, interaction and world state.
- **Renderer** — Godot 3D scene, materials, lighting, camera and effects.
- **Game State** — authoritative runtime state, flags, inventory, player state and systemic consequences.
- **Mission Engine** — objectives, triggers, consequences and mission state.
- **Terminal Engine** — fictional filesystem/network and command parser, isolated from the host OS.
- **Dialogue Engine** — conversations, branching and flags.
- **AI Director** — narrative/systemic threat reactions, not real AI model control.
- **Persistence** — save/load seed and progression state.
- **UI** — HUD, terminal/CRT, dialogue and menus.
- **Audio** — ambience, systemic cues, dialogue and world feedback.

## Dependency direction
Presentation nodes should consume authoritative game state rather than own core gameplay state. World generation should produce data/configuration that the runtime can consume without making the generator responsible for rendering. Mission and dialogue systems communicate through explicit state/events. The terminal engine remains a closed simulation and has no host shell, real network, real credentials or real malware/exploit behavior.

The seed is a reproducibility input, not a complete save state. A save must preserve the seed plus the player's persistent world/progression state required to resume the exact game state.

## Procedural world principles
1. Deterministic: the same seed and generation version must reproduce the same generated base world.
2. Bounded first: start with a small test area before implementing streaming/infinite generation.
3. Layered generation: terrain → roads/districts → structures → points of interest → systemic state → encounters.
4. Hand-authored constraints: procedural generation chooses from designed rules/assets rather than producing arbitrary noise.
5. Versioned generation: changes to generation rules must be versioned so future saves can identify their generation format.
6. Gameplay first: generation exists to create interesting exploration and systemic situations, not merely large maps.

## Presentation philosophy
The world should favor simple geometry and strong atmosphere over photorealism. Advanced infrastructure, abandoned systems, lighting, sound and machine activity should create the post-apocalyptic identity. The terminal is the complementary machine-world interface: **humans see the world; machines see the system.**

## Browser and platform strategy
- Develop and profile primarily on native desktop.
- Keep gameplay/data systems independent of rendering-specific code where practical.
- Test Web export early enough to detect unsupported features and performance problems.
- Avoid C# for the foundation because Godot 4 C# Web export is not currently supported.
- Do not introduce third-party rendering/physics engines unless a measured prototype requirement justifies them.

## Local development path
Required foundation commands after the first executable project shell exists:
- Open the project in **Godot 4.7.2 stable**.
- Run the project from the Godot editor for native development.
- Export a Web build from Godot for browser validation.

The exact project path, export presets and command-line automation will be documented by TASK 02 once the executable project shell exists.

## First implementation order
1. Project shell in Godot 4.7.2.
2. Small deterministic seeded 3D test world.
3. Player movement and camera.
4. Basic interaction system.
5. Terminal engine and CRT interface.
6. Mission state machine.
7. Dialogue/Julia.
8. Detection/trace system.
9. Save state containing seed + persistent progression.
10. Vertical-slice loop and polish.

## Explicit non-goals for the foundation
- No infinite world yet.
- No multiplayer.
- No procedural generation of every asset from scratch.
- No real network/hacking behavior.
- No photorealistic rendering pipeline.
- No large open world before the vertical slice is validated.
