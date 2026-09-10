# DEVELOPMENT WORKFLOW — ANONYM_US_<2047>

## The project loop

`ISSUE → PROMPT.md → BRANCH → READ → PLAN → IMPLEMENT → TEST → REVIEW → DOCUMENT → STATUS → PR → MAIN`

### 1. ISSUE
Define one coherent outcome in GitHub Issues.

### 2. PROMPT.md
Translate the issue into an executable, bounded `.md` task prompt under `AGENTS/PROMPTS/`.

### 3. BRANCH
Create a dedicated branch. Never use `main` for normal agent work.

### 4. READ
Read master context, project status, decisions, task prompt and relevant docs/code.

### 5. PLAN
Identify the smallest implementation and verify dependencies/conflicts.

### 6. IMPLEMENT
Change only the assigned scope.

### 7. TEST
Run the required automated/manual verification.

### 8. REVIEW
Check scope, architecture, regressions, safety boundaries and documentation.

### 9. DOCUMENT
Synchronize durable documentation and record important decisions.

### 10. STATUS
Update phase, blockers and next task.

### 11. PR
Open a reviewable pull request into `main`.

### 12. MAIN
After validation/review, merge the approved result into the stable branch.

## Non-negotiable rule
A future agent must be able to understand the current project state from the repository itself. Do not leave essential context only in chat.
