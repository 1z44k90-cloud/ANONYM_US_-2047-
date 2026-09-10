# GAME STATE

## Core state
- player position
- current zone
- inventory
- discovered evidence
- mission progress
- dialogue flags
- trust/relationship flags
- terminal access state
- simulated trace level
- world-event flags

## Narrative flags
Examples:
- `JULIA_TRUST`
- `SYNAPSE_ALERT`
- `DISCOVERED_ORIGIN`
- `ANONYM_US_STATUS`
- `BLACKOUT_ACTIVE`
- `JULIA_REVEAL_READY`

Names are provisional and can change during implementation.

## Rule
One authoritative state object should drive world, missions, terminal and narrative systems. UI must not silently create contradictory state.
