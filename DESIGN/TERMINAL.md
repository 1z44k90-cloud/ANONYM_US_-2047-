# TERMINAL SYSTEM

## Purpose
The terminal is a core gameplay system, not a cosmetic overlay. It lets the player investigate fictional systems and solve puzzles.

## Example commands
- `help`
- `ls`
- `cd`
- `cat`
- `grep`
- `scan`
- `connect`
- `decrypt`
- `status`
- `trace`
- `payload`

## Virtual environment
The terminal operates on a game-defined virtual filesystem and simulated network graph. Nothing is executed by the host operating system.

## Mission design
Commands should reveal clues, change simulated state and create risk. Incorrect actions may increase a fictional trace meter, lock an in-game node, destroy evidence or trigger a pursuit.

## Authenticity
The interface can use realistic terminology and syntax patterns, but all targets, credentials, addresses, payloads and outcomes are fictional and isolated from real systems.
