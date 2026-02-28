# CLAUDE.md

This file provides guidance for AI assistants (such as Claude Code) working with this repository.

## Repository Overview

**hello-world** is a minimal tutorial/learning repository owned by `rafa1239`. It was created to practice foundational Git workflows — making commits, creating branches, and opening pull requests. There is no application code; the sole source file is `README.md`.

## Repository Structure

```
hello-world/
└── README.md   # Project description (the only tracked file)
```

## Commit History Summary

| Commit | Message |
|--------|---------|
| `f5c35e6` | Initial commit |
| `638ceb3` | Explaining why's of the universe. |
| `364e596` | Update README.md (via branch `rafa1239-patch-1`) |
| `a56f0c6` | Merge pull request #1 from rafa1239/rafa1239-patch-1 |

The history reflects deliberate practice: a direct commit, a branch-based commit merged via pull request.

## Branch Strategy

- **`master`** — main/default branch; represents the stable state.
- **Feature branches** — short-lived branches (e.g., `rafa1239-patch-1`) used for changes submitted as pull requests before merging into `master`.
- **`claude/*`** — branches used by AI assistants (Claude Code) for automated tasks. These follow the pattern `claude/<task-description>-<session-id>`.

## Development Workflow

Because this is a learning repository with no build system, tests, or dependencies, the workflow is straightforward:

1. **Branch** — create a feature branch from `master` for any change.
2. **Edit** — make changes to files (currently just `README.md`).
3. **Commit** — write a clear, descriptive commit message in the imperative mood (e.g., `Add installation instructions`).
4. **Push** — push the branch to `origin`.
5. **Pull Request** — open a PR targeting `master`; merge once reviewed.

## Conventions for AI Assistants

- **Do not create unnecessary files.** This repo intentionally contains only `README.md`. Add files only when explicitly requested.
- **Commit messages** should be concise, written in the imperative mood, and describe *what* the change does.
- **Branch naming** for AI-driven work must follow the pattern `claude/<description>-<session-id>` and must be pushed with `git push -u origin <branch-name>`.
- **Never push directly to `master`** without explicit user approval.
- **No build, lint, or test commands exist** for this repository — do not attempt to run them.
- When adding or modifying `README.md`, preserve its casual, tutorial-friendly tone.

## Key Facts

- **Language/Stack:** None (documentation only).
- **CI/CD:** None configured.
- **Dependencies:** None.
- **License:** Not specified.
