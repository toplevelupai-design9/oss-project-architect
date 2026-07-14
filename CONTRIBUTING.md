# Contributing to OSS Project Architect

Thank you for taking the time to contribute! This document explains how to propose changes, the conventions we follow, and what to expect from the review process. By participating, you agree to abide by our [Code of Conduct](./CODE_OF_CONDUCT.md).

## Table of contents

- [Ways to contribute](#ways-to-contribute)
- [Getting started](#getting-started)
- [Branching model](#branching-model)
- [Commit conventions](#commit-conventions)
- [Pull request process](#pull-request-process)
- [Style and quality checks](#style-and-quality-checks)
- [Reporting bugs](#reporting-bugs)
- [Proposing enhancements](#proposing-enhancements)
- [Architecture decisions and RFCs](#architecture-decisions-and-rfcs)
- [Community expectations](#community-expectations)

## Ways to contribute

- Improve documentation, examples, or templates.
- Add or refine prompts in the [prompt library](./prompts/README.md).
- Triage issues and reproduce bugs.
- Review open pull requests.
- Propose new features via an issue before implementing large changes.

## Getting started

1. Fork the repository and clone your fork.
2. Create a topic branch from `main` (see [branching model](#branching-model)).
3. Make your changes with clear, focused commits.
4. Run the local checks described in [style and quality checks](#style-and-quality-checks).
5. Push your branch and open a pull request against `main`.

```bash
git clone https://github.com/<your-username>/oss-project-architect.git
cd oss-project-architect
git checkout -b docs/improve-architecture
```

## Branching model

We use short-lived topic branches merged into `main` via pull request. Name branches using the pattern `<type>/<short-description>`, for example:

- `feat/prompt-library-testing`
- `fix/broken-roadmap-link`
- `docs/clarify-governance`

`main` is always releasable. Direct pushes to `main` are disabled; all changes go through review.

## Commit conventions

We follow [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/). Each commit message has the form:

```text
<type>(optional scope): <description>

[optional body]

[optional footer(s)]
```

Common types:

| Type | Use for |
| --- | --- |
| `feat` | A new feature or capability. |
| `fix` | A bug fix. |
| `docs` | Documentation-only changes. |
| `refactor` | Code changes that neither fix a bug nor add a feature. |
| `test` | Adding or correcting tests. |
| `chore` | Tooling, CI, or maintenance changes. |

Breaking changes must include a `!` after the type/scope or a `BREAKING CHANGE:` footer.

## Pull request process

1. Ensure your branch is up to date with `main`.
2. Fill in the [pull request template](./.github/PULL_REQUEST_TEMPLATE.md) completely.
3. Link the issue your PR resolves (for example, `Closes #123`).
4. Keep PRs focused; smaller PRs are reviewed faster.
5. At least one maintainer approval and passing CI are required before merge.
6. Maintainers squash-merge by default, using a Conventional Commit title.

## Style and quality checks

Documentation and configuration are linted in CI. To reproduce locally:

```bash
# Lint Markdown
npx markdownlint-cli2 "**/*.md"

# Check for broken links
npx markdown-link-check README.md
```

Please fix any warnings before requesting review.

## Reporting bugs

Use the [Bug report](./.github/ISSUE_TEMPLATE/bug_report.yml) template. Include reproduction steps, expected vs. actual behavior, and environment details. Search existing issues first to avoid duplicates.

## Proposing enhancements

Use the [Feature request](./.github/ISSUE_TEMPLATE/feature_request.yml) template. Describe the problem, the proposed solution, and alternatives you considered.

## Architecture decisions and RFCs

Significant or cross-cutting changes should be recorded as an Architecture Decision Record using the [ADR template](./templates/ADR_TEMPLATE.md) under [`docs/adr/`](./docs/adr/README.md). Larger design proposals should use the [RFC template](./templates/RFC_TEMPLATE.md).

## Community expectations

Be respectful, assume good intent, and keep discussions constructive. Maintainers aim to respond to new issues and pull requests within five business days. Thank you for helping make this project better!
