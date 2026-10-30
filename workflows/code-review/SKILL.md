---
name: code-review
description: Review code changes for correctness, regressions, security, maintainability, and scope. Use for diffs, pull requests, or review requests.
---

# Code Review

Review the change, not the author's style preferences.

## Review priorities

1. Correctness and behavioral regressions.
2. Security, privacy, authorization, and input validation.
3. Data integrity, concurrency, and failure handling.
4. Compatibility with supported platforms and versions.
5. Performance issues supported by a plausible workload.
6. Maintainability and consistency with the existing architecture.
7. Tests and missing coverage.

## Method

- Inspect the full diff and enough surrounding code to understand behavior.
- Trace important callers, data flows, and error paths.
- Check whether tests cover the changed behavior and important edge cases.
- Do not flag speculative issues as definite bugs.
- Do not request unrelated refactoring or cosmetic changes unless they obscure correctness.
- Do not modify code during a review unless the user also requests fixes.

## Findings

For each actionable finding, include:
- Severity: critical, high, medium, or low.
- File and relevant method/line.
- Concrete scenario that triggers the issue.
- Impact and a focused suggested correction.

Lead with the most important findings. If no actionable issue is found, say so and mention review limitations. Never claim tests were run unless they were.
