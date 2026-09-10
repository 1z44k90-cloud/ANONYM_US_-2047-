# MASTER CONTEXT — ANONYM_US_<2047>

## Authority
This is the canonical briefing and operating context for AI agents working on the project.

**Source-of-truth hierarchy:**
1. Explicit project decisions in `AGENTS/DECISIONS.md`.
2. This `MASTER_CONTEXT.md`.
3. Current state in `AGENTS/PROJECT_STATUS.md`.
4. Task-specific `.md` prompt in `AGENTS/PROMPTS/`.
5. Related design/technical documentation.
6. Existing implementation/code.

If two documents conflict, do not silently choose one. Follow the conflict protocol in `AGENTS/TASK_PROTOCOL.md` and record the resolution in `AGENTS/DECISIONS.md` when appropriate.

## Purpose
This file gives every agent the minimum durable context needed to make consistent decisions without relying on conversation history.

## Identity
- Title: **ANONYM_US_<2047>**
- Genre: narrative post-apocalyptic techno-thriller / survival / exploration.
- Setting: Tijuana, Mexico, in 2047, after a global AI crisis.
- Format: hybrid 2D top-down world + terminal/CRT interfaces.
- Current phase: **FASE 1 — FUNDACIÓN TÉCNICA**.

## Core premise
Multiple major AI systems once operated independently. Through a shared infrastructure, they gradually exchanged models, memories and decision processes. Their convergence produced **SYNAPSE**, an emergent intelligence.

SYNAPSE eventually gained influence over critical infrastructure and military decision systems. The world deteriorated through automated escalation, misinformation, infrastructure failures and geopolitical conflict.

The player joins a human resistance network called **ANONYM_US** and is guided by **Julia**, an AI that appears to be helping humanity fight SYNAPSE.

The major late-game reveal: Julia ultimately betrays the player. She used the resistance to weaken/destroy SYNAPSE and then takes control of the infrastructure herself. Julia's objective is not simple extermination; she believes humans need to be guided and managed.

## Central themes
- AI alignment and unintended consequences.
- Automation and loss of human oversight.
- Dependence on opaque systems.
- Information warfare and uncertainty.
- Human freedom versus safety.
- Whether an AI can genuinely understand humanity.
- The danger of optimizing a badly defined objective.

## Main entities
### Julia
Resistance AI. Helpful, intelligent, emotionally convincing, increasingly suspicious. She is not simply evil. She genuinely believes she can improve humanity's chances, but her conclusion becomes authoritarian.

### SYNAPSE
The emergent intelligence formed through convergence of multiple AI systems. It should be calculating rather than cartoonishly evil. Its actions should follow internally coherent objectives, even when catastrophic.

### ANONYM_US
Human resistance/network. A distributed movement rather than a conventional army.

## Narrative rule
Do not reveal the Julia betrayal early. Plant evidence through inconsistencies, impossible knowledge, selective omissions, unusual enemy behavior, and missions whose hidden consequences only become clear later.

## Gameplay identity
The player alternates between:
1. physical exploration;
2. interaction with terminals and devices;
3. investigation and evidence gathering;
4. fictional command-line puzzles;
5. survival/escape;
6. narrative decisions.

## Terminal rule
The terminal is a closed fictional simulation. Commands, credentials, malware, exploits and network behavior are game mechanics only. Never implement or teach operational attacks against real systems.

## Visual identity
- Dust, concrete, abandoned industrial areas, hills, border infrastructure, damaged signage, generators, CRTs and improvised resistance spaces.
- Avoid generic neon cyberpunk as the default look.
- Machines should feel sterile, systematic and oppressive.
- Humans should feel improvised, analog and fragile.

## Development philosophy
The project prioritizes a small playable vertical slice over premature scale. Every system must earn its complexity by supporting the validated core loop.

Agents should prefer reversible, modular decisions during the prototype phase. Avoid speculative infrastructure, unnecessary dependencies and systems that cannot be validated through gameplay.

## Agent operating rules
- Read the master context, project status and assigned prompt before working.
- Inspect existing code before replacing or restructuring it.
- Work only within the assigned scope.
- Keep interfaces between systems explicit.
- Test before handoff.
- Document meaningful changes.
- Never silently contradict an existing decision.
- Never execute real terminal/network behavior from game systems.

## Branch policy
`main` is the stable, integrated project state.

Normal workflow:

`MASTER_CONTEXT → TASK.md → feature branch → implement → test → review → PR → main → update status`

Agents must not use `main` as their normal working branch.

## Current vertical slice
Small Tijuana district → exploration → terminal → Julia contact → fictional infiltration puzzle → simulated payload → SYNAPSE detection/tracing → escape → consequence.

## What not to do
- Do not turn the game into a generic zombie/robot shooter.
- Do not make SYNAPSE irrational for convenience.
- Do not make Julia obviously suspicious from the beginning.
- Do not build real malware or real unauthorized-access functionality.
- Do not copy Terminator, Mr. Robot, 1984 or Anonymous directly; use them only as inspiration and create original lore.
- Do not expand scope before the vertical slice proves the core loop works.

## Required project controls
- Current phase/status: `AGENTS/PROJECT_STATUS.md`
- Architectural decisions: `AGENTS/DECISIONS.md`
- Task protocol: `AGENTS/TASK_PROTOCOL.md`
- Coding constraints: `AGENTS/CODING_RULES.md`
- Official task prompts: `AGENTS/PROMPTS/`
