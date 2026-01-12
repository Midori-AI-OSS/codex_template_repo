# Repository Contributor Guide

This template provides a baseline set of practices for repositories that use a `.codex` directory for contributor coordination. Update and extend these instructions to match your project's tooling, review process, and communication style before onboarding new contributors.

---

## Where to Look for Guidance
- **`.feedback/`**: Planning notes, priorities, and stakeholder feedback. Treat these files as read-only unless you are explicitly asked to maintain them.
- **`.codex/`**:
  - `instructions/`: Process notes, mode-specific guidance, and service-level conventions. Keep these synchronized with the latest decisions.
  - `implementation/`: Technical documentation that accompanies code changes. Update these files whenever behavior or architecture shifts.
  - Other subfolders (e.g., `tasks/`, `brainstorms/`, `prompts/`) capture active work, ideation, and reusable assets. Follow each folder's README or local `AGENTS.md` for details.
- **`.github/`**: Automation, workflow configuration, and repository-wide policy files.
- Additional directories may include their own `AGENTS.md`. Those files take precedence for the directory tree they reside in.

---

## Development Basics
- Set up the project's runtime environment before modifying files. Document the preferred toolchain in `.codex/instructions/`.
- Verification-first: confirm current behavior in the codebase before changing code; reproduce/confirm the issue (or missing behavior); verify the fix with clear checks.
- No broad fallbacks: do not add “fallback behavior everywhere”; only add a narrow fallback when the task explicitly requires it, and justify it.
- No backward compatibility shims by default: do not preserve old code paths “just in case”; only add compatibility layers when the task explicitly requires it.
- Minimal documentation, minimal logging: prefer reading code and docstrings; do not add docs/logs unless required to diagnose a specific issue or prevent a crash.
- Do not update `README.md`.
- Run linters, tests, and any required quality gates that apply to your contribution. Record new commands in `.codex/implementation/` so others can reproduce your results.
- Keep code, configuration, and documentation changes in sync. When you update behavior, review nearby docs for accuracy.
- Use structured commit messages such as `[TYPE] Concise summary` and keep pull request descriptions short and outcome focused.
- Break large efforts into reviewable commits or tasks. Reference related issues, design docs, or feedback files directly in your commits and PRs.
- Respect repository style guides. If none exist yet, document agreed-upon conventions in `.codex/instructions/` and link them here.

---

## Task and Planning Etiquette
- Place actionable work items in `.codex/tasks/` using unique filename prefixes (for example, generate a short hex string with `openssl rand -hex 4`).
- Move completed items into a dedicated archive such as `.codex/tasks/done/` to keep the active queue focused.
- Capture brainstorming notes, prompt drafts, audits, and reviews in their dedicated `.codex/` subdirectories so future contributors can trace decisions.

---

## Communication
- Announce when you start, pause, or complete work using your team's preferred communication command or channel. Replace this sentence with the exact command (e.g., `./contact.sh`) once it is defined for the repository.
- Summarize significant updates in commit messages, pull requests, or planning docs so other contributors can follow the thread of work.

---

## Contributor Modes
This template ships with several baseline contributor modes. Review the matching file in `.codex/modes/` before beginning a task and keep your personal cheat sheet in `.codex/notes/` up to date.

- **Task Master Mode** (`.codex/modes/TASKMASTER.md`)
- **Manager Mode** (`.codex/modes/MANAGER.md`)
- **Coder Mode** (`.codex/modes/CODER.md`)
- **Reviewer Mode** (`.codex/modes/REVIEWER.md`)
- **Auditor Mode** (`.codex/modes/AUDITOR.md`)
- **Blogger Mode** (`.codex/modes/BLOGGER.md`)
- **Brainstormer Mode** (`.codex/modes/BRAINSTORMER.md`)
- **Prompter Mode** (`.codex/modes/PROMPTER.md`)
- **Storyteller Mode** (`.codex/modes/STORYTELLER.md`)

Add or remove modes as needed for your project, and ensure each has a corresponding cheat sheet under `.codex/notes/` for quick reference.

---

## Customizing This Template
1. Replace placeholder text (like the communication guidance above) with project-specific instructions.
2. Populate `.codex/tasks/`, `.codex/instructions/`, and `.codex/implementation/` with initial examples so contributors understand expectations.
3. Document any required tooling, CI commands, or environment setup steps in `README.md` and cross-reference them here.
4. Encourage every contributor to read their mode guide and acknowledge updates whenever this file changes.
