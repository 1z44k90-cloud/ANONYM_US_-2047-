# TASK PROTOCOL

1. Read `AGENTS/MASTER_CONTEXT.md`.
2. Read the issue and the documentation directly related to the task.
3. Inspect existing code before proposing replacements.
4. Define the smallest useful implementation.
5. Keep fictional terminal/network systems isolated from real-world execution.
6. Implement and test the change.
7. Update relevant documentation if behavior or design changed.
8. Report what changed, what was tested, and what remains.

## For multi-agent work
- One agent owns one coherent area at a time.
- Avoid simultaneous edits to the same files unless coordinated.
- World, narrative, terminal, UI and core systems should communicate through explicit interfaces/state rather than hidden coupling.
- When an architectural conflict appears, stop and document the decision before expanding the implementation.

## Definition of done
A task is not complete merely because code exists. It should be understandable, playable/testable where applicable, documented when necessary, and consistent with the master context.
