# Codex Contributor Template

This repository provides a reusable `AGENTS.md` and a baseline set of contributor mode guides under `.codex/modes/`. Copy these files into a new project to bootstrap consistent collaboration workflows without inheriting project-specific tooling rules.

## How to Use This Template
1. Create or choose the target repository you want to prepare for Codex-style collaboration.
2. Clone that repository locally.
3. Copy `AGENTS.md` from this template into the root of the target repository.
4. Copy the `.codex/modes/` directory into the target repository (create `.codex/` first if it does not exist).
5. Review each mode file and replace placeholder or generic language with project-specific expectations.
6. Update the target repository's `README.md`, `.codex/instructions/`, and `.codex/tasks/` so they align with the imported guidance.
7. Commit the changes in the target repository and share the updated instructions with your team.

## Example Self-Prompt
Use a prompt like the following when you want to bootstrap a new repository with this template:

```md
Clone the Codex Contributor Template (https://github.com/Midori-AI-OSS/codex_template_repo.git) repo into a new clean temp folder,
copy its `AGENTS.md` and `.codex/modes` folder into this current project, then customize the instructions to match the project's tooling and workflow.
```

Adapt the wording to match your workflow automation tooling or assistant. The key steps are: clone, copy, customize, and document.

## Customization Checklist
- [ ] Document the team's communication command or channel in `AGENTS.md`.
- [ ] Link to any language- or framework-specific setup instructions in `.codex/instructions/`.
- [ ] Add cheat sheets for each active contributor mode under `.codex/notes/`.
- [ ] Remove unused mode files or add new ones as your project requires.
- [ ] Keep `.codex/tasks/`, `.codex/implementation/`, and `.codex/instructions/` synchronized with ongoing work.

Keep this repository untouched after copying so it remains a clean starting point for future projects.
