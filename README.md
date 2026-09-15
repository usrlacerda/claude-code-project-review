# Claude Code Project Review Skill

A small, reusable Claude Code skill for reviewing software projects before implementation or release.

## What it does

The skill helps Claude:

- inspect a project structure;
- identify missing documentation and tests;
- detect configuration and security risks;
- review code quality and maintainability;
- produce a prioritized action list;
- avoid changing files unless explicitly requested.

## Installation

Copy `.claude/skills/project-review` into your project's `.claude/skills/` directory.

## Usage

In Claude Code, ask:

> Review this project using the project-review skill.

Or:

> Run a project review and prioritize the top 10 improvements.

## Output

The review is organized into:

1. Critical issues
2. High-priority improvements
3. Medium-priority improvements
4. Optional improvements
5. Recommended next steps

## Design principles

- Read before changing.
- Never invent test results.
- Clearly separate facts from recommendations.
- Protect secrets and sensitive configuration.
- Prefer small, reversible changes.

## License

MIT
