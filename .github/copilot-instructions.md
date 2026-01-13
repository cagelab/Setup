---
description: "GitHub Copilot instructions for this repo"
---

## Repo guidance

Follow the repository rules in [AGENTS.md](../AGENTS.md) for all automated changes.

In particular:

- Shell scripts (`*.sh`, `*.zsh`): follow the zsh/shell conventions and keep scripts idempotent.
- Ansible (`*.yml`, `*.yaml`): use 2-space indentation (no tabs), prefer `ansible.builtin.*`, and keep tasks idempotent.

## Additional instruction files

Also follow any scoped rules in `.github/instructions/` (they apply by file glob).

## Repo-specific workflow note

If you change files that are expected to be symlinked into place, run `./makelinks.sh` so the updated versions are actually used.
