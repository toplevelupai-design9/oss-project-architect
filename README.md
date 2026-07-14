# OSS Project Architect

> A production-ready blueprint and toolkit for designing, launching, and maintaining high-quality open-source projects.

[![CI](https://github.com/toplevelupai-design9/oss-project-architect/actions/workflows/ci.yml/badge.svg)](https://github.com/toplevelupai-design9/oss-project-architect/actions/workflows/ci.yml)
[![Docs Link Check](https://github.com/toplevelupai-design9/oss-project-architect/actions/workflows/link-check.yml/badge.svg)](https://github.com/toplevelupai-design9/oss-project-architect/actions/workflows/link-check.yml)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](./LICENSE)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](./CONTRIBUTING.md)
[![Conventional Commits](https://img.shields.io/badge/Conventional%20Commits-1.0.0-fe5196.svg)](https://www.conventionalcommits.org)

OSS Project Architect gives maintainers a batteries-included foundation for running a healthy open-source project. Instead of copy-pasting boilerplate from a dozen repositories every time you start something new, you get a coherent, opinionated set of governance documents, reusable templates, worked examples, automated quality gates, and an **AI prompt library** for the repetitive parts of maintenance.

## Why this exists

Most open-source projects fail for non-technical reasons: unclear scope, missing contribution guidelines, inconsistent reviews, slow triage, and burned-out maintainers. This repository codifies the practices that keep projects sustainable so you can focus on the code that makes your project unique.

- **Start fast.** Drop-in documents and templates that are ready on day one.
- **Stay consistent.** Conventional Commits, ADRs, and RFCs keep decisions traceable.
- **Scale gracefully.** Governance, roadmap, and security policies that grow with your community.
- **Automate the boring parts.** CI, linting, link checking, and a curated prompt library for triage, review, and release notes.

## What's inside

| Area | Description |
| --- | --- |
| `docs/` | Architecture, project specification, roadmap, governance, and Architecture Decision Records. |
| `examples/` | Worked examples showing how to apply the blueprint to a real project. |
| `templates/` | Reusable RFC, ADR, and release-notes templates. |
| `prompts/` | An AI prompt library for triage, code review, changelog and release-notes generation, and documentation. |
| `.github/` | Issue templates, pull request template, CODEOWNERS, Dependabot, and CI workflows. |

## Repository structure

```text
.
├── README.md
├── LICENSE
├── CONTRIBUTING.md
├── CODE_OF_CONDUCT.md
├── SECURITY.md
├── CHANGELOG.md
├── docs/
│   ├── architecture.md
│   ├── project-specification.md
│   ├── roadmap.md
│   ├── governance.md
│   ├── glossary.md
│   └── adr/
├── examples/
├── templates/
├── prompts/
└── .github/
    ├── ISSUE_TEMPLATE/
    ├── workflows/
    └── PULL_REQUEST_TEMPLATE.md
```

## Quick start

1. **Use this repository as a template** (or clone it) for your new project.
2. Search and replace the placeholder owner/repo (`toplevelupai-design9/oss-project-architect`) with your own coordinates.
3. Edit [`docs/project-specification.md`](./docs/project-specification.md) to define your goals and scope.
4. Review [`docs/roadmap.md`](./docs/roadmap.md) and adjust the milestones.
5. Enable the workflows under [`.github/workflows/`](./.github/workflows) and set up branch protection.
6. Start triaging and reviewing with the [prompt library](./prompts/README.md).

```bash
git clone https://github.com/toplevelupai-design9/oss-project-architect.git
cd oss-project-architect
```

## Using the prompt library

The [`prompts/`](./prompts/README.md) directory contains copy-paste prompts for common maintainer workflows:

- [Issue triage](./prompts/issue-triage.md)
- [Pull request review](./prompts/pr-review.md)
- [Changelog generation](./prompts/changelog-generation.md)
- [Release notes](./prompts/release-notes.md)
- [Documentation writing](./prompts/documentation-writer.md)
- [Commit messages](./prompts/commit-message.md)

Each prompt documents its intent, required inputs, and expected output so results are consistent across maintainers and tools.

## Documentation

- [Architecture](./docs/architecture.md)
- [Project specification](./docs/project-specification.md)
- [Roadmap](./docs/roadmap.md)
- [Governance](./docs/governance.md)
- [Glossary](./docs/glossary.md)
- [Architecture Decision Records](./docs/adr/README.md)

## Contributing

Contributions are welcome and appreciated. Please read the [Contributing Guide](./CONTRIBUTING.md) and our [Code of Conduct](./CODE_OF_CONDUCT.md) before opening an issue or pull request. Good first issues are labeled [`good first issue`](https://github.com/toplevelupai-design9/oss-project-architect/labels/good%20first%20issue).

## Roadmap

See [`docs/roadmap.md`](./docs/roadmap.md) for planned milestones and how to influence them.

## Security

Found a vulnerability? Please follow the responsible-disclosure process in [`SECURITY.md`](./SECURITY.md). Do not open a public issue for security reports.

## License

Distributed under the [MIT License](./LICENSE). © 2026 Hosein Bagheri.
