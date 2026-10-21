# Prism Unlocked agent guidance

## Project overview

Prism Unlocked is a community fork of Prism Launcher for managing Minecraft instances. It is primarily a CMake and C++/Qt project, with Java launcher support under `libraries/launcher`.

## Working rules

- Preserve existing user changes and inspect `git status` before editing.
- Keep changes focused on the requested behavior.
- Use `apply_patch` for source and documentation edits.
- Do not change upstream attribution or licensing notices unless the task explicitly requires it.
- Treat generated build output as disposable; do not commit it.
- When changing product identity, check CMake, installer, desktop integration, URL schemes, and documentation together.

## Validation

- Prefer the repository's CMake preset for the target platform.
- Build the affected target after CMake or packaging changes.
- Run relevant tests with `ctest` when a configured build is available.
- For documentation-only changes, verify Markdown structure and search for stale names.

## AI-assisted work

AI tools may assist development, but every generated suggestion must be reviewed by a human maintainer. AI-assisted contributions must disclose the tool used and its role, as described in `CONTRIBUTING.md`.
