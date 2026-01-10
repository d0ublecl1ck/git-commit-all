# Git Commit All

A Codex skill that enforces a strict, safe workflow for committing all relevant changes in a repo.

## What it does

- Runs pre-commit checks in parallel: `git status`, `git diff`, `git log --oneline -5`
- Adds only relevant untracked files (no unrelated files)
- Commits with a HEREDOC message (no signatures, no push)
- Re-commits if pre-commit hooks modify files

## When to use

Use when you want Codex to commit all relevant changes without extra confirmations, following a strict workflow and safety rules.

## Installation

Copy the skill folder into your Codex skills directory (example for macOS/Linux):

```bash
cp -R git-commit-all ~/.codex/skills/custom/
```

## Notes

- This skill never modifies git config
- This skill never pushes unless explicitly requested
