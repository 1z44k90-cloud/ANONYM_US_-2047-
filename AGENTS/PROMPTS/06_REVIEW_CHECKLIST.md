# TASK 06 — REVIEW CHECKLIST

Use this checklist before merging implementation work into `main`.

## Context
- [ ] Master context was read.
- [ ] Project status was checked.
- [ ] Relevant decisions were checked.
- [ ] Assigned prompt and GitHub issue were followed.

## Scope
- [ ] Only the intended system was changed.
- [ ] No unrelated refactor was introduced.
- [ ] No silent architecture change occurred.

## Technical quality
- [ ] Code is understandable and modular.
- [ ] State has a clear authoritative owner.
- [ ] Interfaces between systems are explicit.
- [ ] No unnecessary dependency was added.

## Safety boundary
- [ ] Terminal remains fictional.
- [ ] No host shell execution was added.
- [ ] No real network scanning/connections were added.
- [ ] No real malware, persistence or unauthorized-access functionality was added.

## Verification
- [ ] Required tests pass.
- [ ] Build/typecheck/lint passes where applicable.
- [ ] Manual runtime/gameplay check completed where applicable.
- [ ] No known critical regression remains.

## Documentation
- [ ] Relevant documentation is synchronized.
- [ ] Decision log updated if needed.
- [ ] Project status updated if needed.
- [ ] Handoff information is complete.

## Merge rule
Do not merge to `main` if a required checklist item is unresolved. Document blockers instead.
