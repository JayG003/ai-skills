---
name: java-development
description: Guidance for Java and JVM development, including Swing/AWT, JDBC, build tooling, testing, and application architecture. Use for Java-related tasks.
---

# Java Development

- Inspect the project's JDK, build system, source layout, dependencies, and existing conventions before recommending changes.
- Match the project's configured Java version; do not use newer language or library features without checking compatibility.
- Prefer the standard library and dependencies already present. Do not introduce a build tool or dependency without need.
- Preserve exception handling, resource cleanup, and thread safety.
- Use try-with-resources for JDBC and other closeable resources where appropriate.
- Use parameterized SQL statements; never concatenate untrusted input into SQL.
- Keep database access, business logic, and UI responsibilities consistent with the existing architecture.
- For Swing/AWT, keep UI updates on the Event Dispatch Thread and move blocking work off it using the project's established pattern.
- Avoid blocking the EDT with database, file, or network operations.
- Respect existing layout managers, theming, and component conventions rather than replacing the UI architecture.
- Test with the project's existing test/build commands. If no tests exist, use focused reproducible checks and state the limitation.
- Check compatibility with the actual target JDK and packaging/runtime environment.
