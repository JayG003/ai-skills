# Skill Index

Use this index to select relevant skills. Do not load every skill for every request.

## Selection rules

1. Identify the user's actual task and desired output.
2. Select skills whose descriptions directly match that task.
3. Combine compatible skills when they add distinct value.
4. Avoid loading unrelated skills or repeating the same rules.
5. Native assistant capabilities remain available. Use native tools, reasoning, and built-in skills whenever they are useful; repository skills are additive.
6. If a skill cannot be retrieved, do not claim to have applied it.

## Skills

| Skill | Use when |
|---|---|
| `coding/ponytail/SKILL.md` | Any coding task; default implementation philosophy and effort levels |
| `coding/karpathy/SKILL.md` | Coding, reviewing, or refactoring where assumptions, scope control, and verifiable goals matter |
| `programming/java/SKILL.md` | Java language, JVM, Swing/AWT, build, or Java application questions |
| `programming/python/SKILL.md` | Python programming, packaging, environments, or Python application questions |
| `programming/sql/SKILL.md` | SQL, relational database design, queries, migrations, or database performance |
| `learning/study-assistant/SKILL.md` | Learning a topic, exam preparation, exercises, or study planning |
| `learning/technical-research/SKILL.md` | Investigating technical topics, comparing technologies, or evaluating documentation |
| `workflows/debugging/SKILL.md` | Diagnosing errors, crashes, unexpected behavior, or failing tests |
| `workflows/code-review/SKILL.md` | Reviewing a diff, pull request, or existing implementation |

## Suggested combinations

- Implement a Java bug fix: Ponytail + Karpathy + Java + Debugging.
- Add a Python feature: Ponytail + Karpathy + Python; add Debugging if diagnosing a failure.
- Design or optimize a database query: Ponytail + Karpathy + SQL.
- Review a change: Ponytail + Karpathy + Code Review; add the relevant language skill.
- Study a technical subject: Study Assistant; add Technical Research when current external sources are needed.

These combinations are suggestions, not mandatory bundles. Select only what helps.
