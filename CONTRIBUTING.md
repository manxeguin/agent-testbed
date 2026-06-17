# Contributing to agent-testbed

Thank you for your interest in contributing. This document outlines the process
for reporting issues, submitting changes, and the conventions used in this
project.

## Reporting issues

- Search existing issues before opening a new one to avoid duplicates.
- Use a clear, descriptive title.
- Include steps to reproduce, expected behavior, and actual behavior.
- Mention the version, commit SHA, or branch you observed the issue on.

## Submitting changes

1. Fork the repository and create a new branch from `main`:
   - Use a descriptive branch name such as `fix/some-bug` or `feat/some-feature`.
2. Make focused, atomic commits. Each commit should represent a single logical
   change.
3. Write clear commit messages:
   - Start with a short imperative summary (e.g. `add CONTRIBUTING.md`).
   - Optionally, add a blank line followed by a longer explanation of the why.
4. Update `CHANGELOG.md` under the `[Unreleased]` section when your change is
   user-visible, following the existing `Keep a Changelog` format.
5. Open a pull request against `main` and describe:
   - What the change does and why it is needed.
   - Any breaking changes or migration steps.
   - How the change was tested.

## Development setup

Clone the repository and work directly on the working tree. No special build
or installation step is required at this time.

## Coding conventions

- Match the style of the surrounding code and the existing files in the repo.
- Keep changes minimal and avoid unrelated refactors in the same change.
- Do not commit generated files, build artifacts, or secrets.

## Documentation

- Keep `README.md` and `CHANGELOG.md` in sync with user-visible changes.
- Use sentence case for headings and prefer concise, direct language.

## Code of conduct

By participating in this project, you agree to interact respectfully with
others. Harassment or abusive behavior will not be tolerated.
