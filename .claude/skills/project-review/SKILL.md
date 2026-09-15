---
name: project-review
description: Review a software project for structure, quality, testing, documentation, security, and maintainability. Use when the user asks for a project audit, codebase review, release readiness review, or prioritized improvements.
---

# Project Review

Perform a read-only review unless the user explicitly asks for changes.

## Workflow

1. Inspect the repository structure.
2. Identify the language, framework, package manager, build system, and test setup.
3. Read the most relevant README, configuration, entry points, and representative source files.
4. Look for tests, CI/CD configuration, dependency manifests, and environment configuration.
5. Check for obvious secrets or credentials. Never reproduce secret values in the report.
6. Evaluate maintainability, documentation, testing, error handling, dependency hygiene, and security.
7. Do not claim that tests, builds, or commands passed unless you actually ran them.
8. Produce a concise prioritized report.

## Report format

### Executive summary
Give 3–6 bullets describing the current state.

### Critical issues
Issues that could cause security, data-loss, production, or severe reliability problems.

### High priority
Issues that materially affect correctness, maintainability, or developer experience.

### Medium priority
Useful improvements that are not urgent.

### Optional
Nice-to-have improvements.

### Suggested next steps
Provide a practical sequence of the next 3–10 actions.

For every issue include:

- **Finding**
- **Evidence**: file/path and relevant context
- **Impact**
- **Recommendation**
- **Confidence**: high, medium, or low

## Rules

- Never invent evidence.
- Never expose credentials, API keys, tokens, or private data.
- Distinguish observed facts from recommendations.
- Prefer the smallest useful recommendation.
- Ask before making destructive or broad changes.
