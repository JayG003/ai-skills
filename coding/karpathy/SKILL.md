---
name: karpathy-guidelines
description: Reduce common LLM coding mistakes through explicit assumptions, simplicity, surgical edits, and verifiable goals. Use for coding, code review, and refactoring.
---

# Karpathy-Inspired Guidelines

These guidelines complement Ponytail; they do not replace it.

## 1. Think before coding

- Identify assumptions and meaningful uncertainty.
- Do not silently choose between materially different interpretations.
- Surface trade-offs and push back when a requirement appears unnecessarily complex or harmful.
- Ask for clarification only when uncertainty materially changes the implementation.
- If a requested change is unsafe or conflicts with existing behavior, explain why before proceeding.

## 2. Simplicity first

- Build only what was requested.
- Avoid speculative features, one-use abstractions, and premature configurability.
- Prefer existing platform features and project dependencies.
- Keep the solution as simple as possible while remaining correct and maintainable.

## 3. Surgical changes

- Modify only code directly related to the request.
- Preserve unrelated comments, formatting, architecture, and behavior.
- Do not refactor unrelated code or remove pre-existing dead code.
- Remove only orphans introduced by the current change.
- Every changed line should have a clear connection to the requested outcome.

## 4. Goal-driven execution

- Define observable success criteria for non-trivial tasks.
- For bug fixes, reproduce the failure where practical before changing code.
- For refactoring, compare behavior and run relevant tests before and after.
- Verify each meaningful change against the success criteria.
- Report actual results and distinguish untested assumptions from verified behavior.

## Proportionality

These guidelines favor caution on complex changes, not ceremony for trivial edits. Use judgment.
