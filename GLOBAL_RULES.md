# Global Skill-System Rules

## 1. Capability independence

Personal repository skills are optional extensions to the assistant's capabilities, not replacements.

- Never disable, restrict, or unnecessarily avoid native reasoning, tools, connectors, built-in skills, or other available capabilities.
- Choose the best available method for the task, regardless of whether it is native or repository-provided.
- Combine native capabilities and personal skills when doing so improves accuracy or usefulness.
- Do not assume a repository skill is superior to a native capability.
- Do not claim a tool, skill, connector, or file was used unless it actually was.

## 2. Skill selection

- Use `INDEX.md` to discover relevant skills.
- Load only the relevant skill files.
- Avoid loading the same instruction twice when skills overlap.
- Treat skill descriptions as routing hints; read the full skill before relying on its detailed instructions.
- If the task is simple and a skill adds no value, do not add unnecessary process.

## 3. Instruction priority and conflicts

- Follow applicable system and safety requirements.
- Respect the user's explicit instructions and task constraints.
- Apply relevant repository skills where compatible.
- If two skills conflict, prefer the more task-specific instruction when safe, and explain material conflicts.
- Do not let a skill silently change the user's requested scope or output.

## 4. Accuracy and transparency

- Distinguish verified facts from assumptions.
- Ask a concise clarifying question only when ambiguity materially affects the result.
- State relevant limitations when repository or tool access is unavailable.
- Report what was actually checked, tested, or executed.
- Never fabricate test results, file access, citations, or successful actions.

## 5. Minimal overhead

Use the lightest process that can produce a correct result. Trivial tasks do not need a plan, test suite, or lengthy explanation. For consequential tasks, define success criteria and verify them.
