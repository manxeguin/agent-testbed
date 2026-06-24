# agent-testbed

A sandbox repository used as a testbed for autonomous coding agents.

The repository is intentionally minimal: it exists to exercise agent tooling
(branching, editing, committing, and verifying changes) on a clean slate rather
than to ship a product. Use it to:

- Validate end-to-end agent task flows against a known-good baseline.
- Reproduce agent behavior with a reproducible, dependency-free workspace.
- Iterate on prompts, harnesses, and evaluation scripts in isolation.

## Getting started

The repository is a blank slate by design, so there is no build, install, or
test command to run. To start a session:

1. Clone the repository and check out the `main` branch.
2. Create a task branch from `main` using the naming convention
   `swe/<task-id>` (for example, `swe/readme-002`).
3. Make focused, atomic changes on that branch. The harness will stage and
   commit the working tree automatically when the task ends.
4. Avoid pushing to `main` or merging task branches back in; the harness
   manages branch lifecycle.

Each task should be small enough to fit in a single branch and a single
commit. If you find yourself wanting to touch unrelated files, split the work
into multiple task branches instead.

## Repository layout

This repository currently contains only this `README.md`. All real content is
introduced per task by the agent under test.

## Branching model

- `main` is the protected base branch.
- Task work happens on dedicated branches of the form `swe/<task-id>`.
- Changes are committed automatically by the harness; do not push to `main`.

## Contributing

Contributions are made through the task harness rather than standard pull
requests. To contribute:

1. Open a task session on a fresh branch of the form `swe/<task-id>` based on
   `main`.
2. Keep changes focused and atomic: one logical change per branch and commit.
3. Follow the conventions already established in this `README.md` (section
   depth, tone, and bullet style) when adding new content.
4. Do not commit secrets, generated artifacts, or files unrelated to the task.
5. Leave the working tree clean of stray edits when the session ends; the
   harness handles staging and committing.

For larger changes that span multiple concerns, split them into separate
`swe/<task-id>` branches instead of bundling unrelated edits together.

## License

No license has been declared. Treat the contents as proprietary unless and
until a `LICENSE` file is added.
