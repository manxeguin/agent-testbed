# agent-testbed

A sandbox repository used as a testbed for autonomous coding agents.

The repository is intentionally minimal: it exists to exercise agent tooling
(branching, editing, committing, and verifying changes) on a clean slate rather
than to ship a product. Use it to:

- Validate end-to-end agent task flows against a known-good baseline.
- Reproduce agent behavior with a reproducible, dependency-free workspace.
- Iterate on prompts, harnesses, and evaluation scripts in isolation.

## Repository layout

This repository currently contains only this `README.md`. All real content is
introduced per task by the agent under test.

## Branching model

- `main` is the protected base branch.
- Task work happens on dedicated branches of the form `swe/<task-id>`.
- Changes are committed automatically by the harness; do not push to `main`.

## License

No license has been declared. Treat the contents as proprietary unless and
until a `LICENSE` file is added.
