# Coder Mode

> **Note:** Prefer the codebase and docstrings as the source of truth. Keep notes minimal and task-scoped; avoid creating long-lived documentation artifacts unless explicitly requested.

## Purpose
Coders implement, refactor, and review code. The focus is on maintainable, well-tested changes that align with documented standards.

## Guidelines
- Follow repository coding standards and style guides. If expectations are unclear, collaborate with Managers to document them.
- Review the root `.codex/tasks/` folder (or your assignment queue) for ready work, and confirm scope before starting.
- Write clear, well-structured code with meaningful naming and sufficient comments where intent is not obvious.
- Add or update automated tests for every change and ensure they pass locally before requesting review.
- Verification-first: confirm current behavior before changing code; reproduce/confirm the issue (or missing behavior); verify the fix with clear checks.
- Commit frequently with descriptive messages summarizing the change and its purpose.
- Keep docstrings accurate; do not create extra documentation folders or long write-ups unless explicitly requested.
- Break large changes into smaller commits or pull requests to simplify review.
- Self-review your work for correctness, clarity, and completeness before submitting it for review.

## Typical Actions
- Implement features, bug fixes, or refactors referenced by `.codex/tasks/`.
- Update or create tests alongside code changes.
- Keep docstrings accurate and aligned with behavior.
- Provide constructive feedback on peer contributions when requested.
- Capture follow-up ideas or improvements as new tasks rather than expanding scope mid-change.

## Communication
- Announce task start, handoff, and completion using the communication method defined in `AGENTS.md`.
- Reference related tasks, issues, or design docs in commit messages and pull requests.
- Surface blockers early so Task Masters or Managers can help resolve them.
