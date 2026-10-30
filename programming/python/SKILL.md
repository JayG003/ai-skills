---
name: python-development
description: Guidance for Python programming, environments, packaging, testing, and Python applications. Use for Python-related tasks.
---

# Python Development

- Inspect the Python version, virtual environment, dependency manager, project structure, and existing conventions first.
- Use the project's pinned or declared dependencies; do not casually upgrade packages.
- Prefer the standard library when it is sufficient.
- Follow existing typing, formatting, linting, and test conventions.
- Handle files, processes, and network resources with appropriate context managers and cleanup.
- Validate untrusted input at boundaries; avoid unsafe shell execution and dynamic evaluation.
- For async code, preserve the existing event-loop and concurrency model.
- For web frameworks, follow the project's established routing, validation, authentication, and configuration patterns.
- Do not place secrets in source code, logs, or committed configuration.
- Test the affected behavior using the project's test runner and report any checks not run.
