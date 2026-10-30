---
name: debugging
description: Systematically diagnose bugs, errors, crashes, and failing tests. Use when the user reports unexpected behavior or asks to troubleshoot.
---

# Debugging Workflow

1. **Capture the failure:** Obtain the exact error, stack trace, logs, steps to reproduce, environment, and expected versus actual behavior. Ask only for missing information that blocks diagnosis.
2. **Inspect before changing:** Review relevant code, configuration, dependencies, recent changes, and callers.
3. **Form a testable hypothesis:** Explain the likely cause and distinguish evidence from guesses.
4. **Reproduce:** Prefer a minimal reproducible case or failing test before editing.
5. **Fix the root cause:** Make the smallest complete change; avoid unrelated cleanup.
6. **Verify:** Run the focused test or reproduction, then relevant regression checks.
7. **Report:** State the cause, changed files/locations, verification results, skipped checks, and remaining risks.

Do not recommend destructive resets, data deletion, or irreversible commands as casual first steps. Explain impact and obtain confirmation where appropriate.
