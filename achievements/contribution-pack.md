# Contribution Pack (Cross-Repo)

This pack standardizes fast, high-quality contribution cycles across personal and external repositories to support Pull Shark, Pair Extraordinaire, and Quickdraw goals.

## 1) Issue template (Quickdraw-ready)
```md
## Summary
[One-line issue statement]

## Scope
- Affected file(s):
- Expected behavior:
- Current behavior:

## Acceptance Criteria
- [ ] Root cause identified
- [ ] Fix applied
- [ ] Validation evidence added
```

## 2) PR template (merge-friendly)
```md
## What changed
- [ ] Focused fix
- [ ] Tests/validation updates
- [ ] Docs/readme update (if needed)

## Why
[Root-cause explanation]

## Validation
- [ ] Local run output attached
- [ ] No regressions observed

## Links
- Issue: #[number]
```

## 3) Co-author workflow (Pair Extraordinaire)
1. Create paired branch and split task into two commit units.
2. Add co-author trailer to at least one merge-bound commit:
```bash
git commit -m "Improve asset validation recursion

Co-authored-by: Partner Name <partner@example.com>"
```
3. Merge through PR so commit enters default branch history.

## 4) Quickdraw execution checklist
1. Open narrowly scoped issue.
2. Implement fix in same workflow window.
3. Link issue in PR, merge quickly, close issue.
4. Capture timestamps and URLs in achievement tracker.

## 5) Validation baseline for personal repos
- `david-on-cloud`: `npm run test:validate`
- `networking-labs`: markdown lint/manual checklist
- `scripting`: run script examples or dry-run command output
